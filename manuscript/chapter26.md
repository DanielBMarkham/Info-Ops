# Appendix A: Creating the Analysis Canvas 

1. Make sure your model is all inside EasyAM and you've run the EasyAM compiler.
2. From the EasyAM GitHub root, download the AnalysisGridTest2 Excel file. 
3. Replace the example Master Model with your own, adding rows as needed.
3. Find a program to make UML diagrams. (Enterprise Architect is recommended but LucidChart will also work. Both can be for free at first).
4. Using the .amout files for each item in your Master Model, create the associated diagrams (Remember for each item there is an .amout with all the linkages and details you could possibly want).
5. These .amout files are also used to create entries in the row that has 
"Behavior to Structure", "Behavior to Supplementals", "Supplementals to Behavior", and "Structure to Behavior" sections.
6. For "Supplementals to Structure", take each Supplemental, on a notepad, write down all the behaviors it participates in. Then for each of those behaviors, list all of the structural items. Join all the lists together. Now you have a list of structure items that can be impacted by this supplemental.
7. For the reverse box, "Structure to Supplementals", use the results from #6.
8. The bottom section, which includes children and outcomes, should also come directly from the .amout cards for each item.

