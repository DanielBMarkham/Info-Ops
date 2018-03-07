# Chapter 14

If you've ever worked with databases, there's a thing called "database normalization". This basically means for any set of data you are collecting about a problem, there's a way to store and use it getting the maximum amount of value using the least amount of space and effort[^14-1]

[^14-1]: Insert long discussion here about document-oriented databases and the NoSQL movement. Sometimes that makes sense -- but database normalization still represents a type of optimizing information gathering and processing.

When you don't have a lot of anything, the way you store it doesn't matter that much. A technology project with a co-located team alongside a real owner and real user that only lasts for a month or two might make do with nothing formal at all -- although I'd still make that master model. Everything hinges off of it, and it's far too useful of a tool (and easy to make) to pass for projects of any size.

But when you're asking a lot of questions and gaining alignment, you can cover a ton of territory. Even if you decide *not* to do something, that might be an important conversation point. I've been known to make a quick list of "excluded behaviors" at the bottom of my master backlog.

And behaviors define the borderlands, the dermarcation point between "stuff we're doing" and "stuff we're not doing". If it's not in our master backlog, we're not doing it.[^14-2]

[^14-2]: I've never done any detail work on anti-behaviors. I guess it's possible. I wouldn't advise it, however. The important thing about anti-behaviors is that they help qualify and add detail to real Master Backlog Items (MBIs). So it's great to note they exist, then figure out what detail you're missing in the MBL, if any, that the anti-behavior points out. Many times they make excellent reminders of conversations that ended with the team deciding something was out of scope. (So while details don't make sense to me, adding notes might be a great idea.)

We've worked out that we've got the minimum set of tags. We've also worked out how to organize things using our tags into pyramids with cross-linking items. This is the minimal system necessary for organizing any analysis data.

But like we said, this stuff gets out of hand quickly. People send us emails with stuff we need to remember, but not right now. There are feature discussions that are important to stuff we delivered six months ago. There are all of these random notes we gathered when we had that weekend user workshop. Information grows like a snowball -- which is one of the reasons the tagging system is so important in the first place. Too much gets lost and/or stuck somewhere it shouldn't be.

So for any project we have that's non-trivial we'll need to store information and recall it. Now that we're moving from theory to application in the book, we'll also start working on larger analysis models and automated collection and processing. 

Do we really need to move to programming? Does every technolog system have to end in some overblown tool? Isn't this just the opposite of what we've been learning all along?

It's a good question. Working by hand with physical items in a group is always best. It creates a situation and a game where the dialectic naturally happens.

When moving data around in databases, programmers have an acronym, **ETL**, which stands for **Extract**, **Transform**, and **Load**. Let's talk about how that applies to us.

First, **Extract** is when we take data from some other place, either a conversation or an datastore somewhere. We've talked about the *real* version of extract, creating a shared mental model while identifying important conversation points for later. There's also extracting information from some datastores. We'll cover that later in this section.

**Transform** is where you move the data from one model to another. Our master models and analysis pyramid that we've created is where everything goes. When we take conversations and **Transform** them, we're **Synchronizing the Model**,making sure that everything refers to everything else. After we do a little nerdy stuff installing a tool, we're going to cover that next, both in manual and automated form.[^14-3]

[^14-3]: Also known as "Grooming the backlog"

Finally, the **Load** stage is where the new information is merged with the older stuff. That's simple once we've got an analysis pyramid and transformed data.

**Transforms always happen manually**. Extracting stuff from various systems to have a good conversation can be manual, but usually involves some kind of tool. Once we've organized stuff and synchronized the model, Loading stuff back into our system can also be done manually, but is best suited for automation.

The important part is the transform, and for that we need the dialectic. Just moving bits and pieces around? We have tools for sorting and filing. We should use them. It's the organization part where the real work happens.

We may have to work with seven-thousand item backlogs (Yes, I've seen them.) We may have thousands of items on a bug list. Our work will be the same as it always was, but there's no point in banging our head against a wall. Since the nature of analysis is always having more data and information than you need to work with at one time, we need to know how to work with lots of data.

So, like it or not, to continue forward we'll need both a tool and a bunch of sample data. We'll also be talking about what can be automated and what can't.

Our pattern will be to talk about the simplicity of the theories involved, then the complexity of the data, then how to combine both and make the data simple in order to physically organize our thoughts as a group. Throughout this we'll be using tools to move data around.

So put on your tin-foil hats and pocket-protectors. We're going to need to get our nerd on. 

![](images/github-easyam.png)

## Downloading and Installing EasyAM

### General Instructions

First, get the latest version of the compiler and sample data files by opening your web browser and going to [https://github.com/DanielBMarkham/easyam](https://github.com/DanielBMarkham/easyam)

Once there, you'll see a green button that says "Clone or Download". Click on that. If you're a programmer and know how to use git, you'll probably clone the repository. Otherwise you'll click on the "Download zip" button to get a zip file of the project.

Once the zip file has been downloaded, extract it into a folder that you can remember. 

![Your directories will look something like this](images/easyam-folders.png)

You should have a bookprog folder. Inside of that you'll have a sample data folder. Inside of that there will be the samples we use.

You will need to have the .NET CLR 4.0 libraries or later installed to run EasyAM. All Windows and most Linux installations already have these available. 

Open a command-line prompt and go to the bookprog folder.

In windows, to see what versions of .NET you have installed, from the command-line prompt type "dir /b /ad /o-n %systemroot%\Microsoft.NET\Framework\v?.*" (Wow, that's easy, right?) You should see lines for 4.0 or greater.

On linux and a Mac, just install the latest version of .NET Core. You'll find instructions for installing .NET Core on your OS at [https://www.microsoft.com/net/core](https://www.microsoft.com/net/core) (Visit the site from the computer you are installing to, since Microsoft determines your computer and routes you to the appropriate place depending on your OS)

I coded EasyAM using Mono, which is the old open-source .NET runtime for linux. (It's a great tool, by the way). That's [here:](http://www.mono-project.com/)

(NOTE TO BETA READERS: In Windows, you'll need to just use the bin/Debug folder for now. In linux, clone the project, then use mono to compile it to a single run-time file, eg "mkbundle -o easyam --deps --static easyam.exe". This will make a file named "easyam" that you can run from the command-line e.g. "./easyam --help")

Once you've got .NET and EasyAM installed, from a command line in the bookprog folder, type "easyam --help". 

You should be looking at help text which includes some sample easyam code.

[](images/easyam-help-text.png)

If you want to use EasyAM in a lot of places, and you probably will, you'll also need to add it to your PATH, so that it will run no matter what directory you are in.

## How Does EasyAM Work?

Once EasyAM is installed, using it is fairly simple:

1. Take mostly freeform text notes using the EasyAM tags.
2. Pick a directory for everybody to use. 
3. Save your notes with an ".amin" extension. (amin stands for Analysis Model IN)
4. Run the EasyAM compiler (Point it to your input directory if you are running it from somewhere else)
5. The compiler goes through all of your .amin files in that directory and its subdirectories *in alphabetical order*
6. Using the tags, it sorts, organizes, collates, and creates all of the pyramids and crosslinks for you
7. It outputs everything in a standardized .amout format. (amout is for Analysis Model, OUT)

Each file starts from a completely blank slate. As you add tags, you indicate where you want to put the information. So if you had some notes to add for the Master Backlog Item "Wiggle When I Walk", you'd start with a fresh file and do it like this:

```
MASTER BACKLOG 
  Wiggle When I Walk 
    NOTES:
      Wiggle in the walk
      Giggle in the talk
      Makes the world go round
      Ain't nothin' in the world 
      Like a big-eyed girl
      That makes me act so funny
```

And so on.

You identify where stuff goes, then put stuff in there.

Indentation is important. In the above example, by moving in another indent level each line, we show that this line goes under the previous one. If I mess up an indent, weird things happen.

Let's say I lost an indent on the last line.

```
MASTER BACKLOG 
  Wiggle When I Walk 
    NOTES:
      Wiggle in the walk
      ...
  That makes me act so funny
```

In this case, I've created a new Master Backlog Item titled "Makes me act so so funny", which is not what I wanted.

The program eats its tail, that is, it outputs in the same format as it inputs, so you can take all of the organized, sorted, and processed amout files and use them as input for another project. 
  
This means we can pipe analysis information from one project to another, or to another online system that reads EasyAM

I always prefix my .amin files with the date in yyyy-mm-dd format along with my initials. So the analysis notes I took on March 1st last year are named "2018-03-01 dbm Initial Notes.amin" This way when EasyAM processes alphabetically, the notes are processed in correct date order.

EasyAM takes source and destination directories as optional parameters. If you provide them, it uses them. Otherwise it uses the current directory. You can also output everything to a single file if you like.

```
./easyam /S:./infiles /D:./outfiles /O:SINGLEFILE=myfile.amout 
```

The above example takes all of the files ending in .amin in the ./infiles directory, processes them alphabetically, then outputs the entire model as one file to ./outfiles/myfile.amout

![Looks like code, feels like code. Using EasyAM in SublimeText](images/sublime-text-extension-example.png)

### It's Programming, Silly

A key concept is that EasyAM works just the same as any other programming tool or language on your system. You can edit files using your IDE, you can version control using DropBox or something like git (for more advanced usages). You can diff two files, you can share common master files and use/maintain your own project-related ones.

If all of this sounds too nerdy for you, if you have DropBox and a small team, create and edit your files in notepad or some text editor and save to a DropBox folder. DropBox will handle all of the moving around, sharing, and versioning for you. If you move past a small team, you should learn to use git and GitHub and save and version your files that way.

For this section, we're going to be talking about working in a small team. (It might be a huge project, but the number of people is small.) So use whatever works for you. Notepad or some other simple text editor will go a long way.

### Keeping Current and Getting Help

To keep current with the progress of EasyAM, which is open source and free, simply visit the GitHub site. GitHub also has a feature where you can watch and be notified when the project changes.

To get assistance or report a bug, send an email to help@easyam.org

Now let's organize some stuff!



