# Homework 8: Capstone

## Objectives

This assignment is designed to help you:
1. Plan and implement a project in computational biology from start to finish
2. Assess and use previously published biological research data
3. Apply reproducible computational tools (both R and Python) to summarize and visualize data to answer research questions
4. Document project progress using version control and a README file

## Summary

For your capstone project, you will select a dataset and identify a series of questions to answer using these data. You will apply coding approaches covered this semester (both R and Python, as well as any other tools you choose to apply) to answer these questions. Your final submission will be a public GitHub repository (`homework08`) containing code, figures, and documentation. You'll submit the URL to your public GitHub repository via Canvas.

Your performance on this assignment will be assessed using the attached [rubric](#rubric) (80 points total). 

## Details 

To complete this project, you should:
1. Choose one of the following datasets. These datasets are all previously published and available through Data Dryad, a public repository. Please see the next section on identifying research questions for additional context in selecting a dataset.
   - Glaucoma diagnosis https://datadryad.org/stash/dataset/doi:10.5061/dryad.q6ft5 
   - Triple negative breast cancer imaging https://datadryad.org/stash/dataset/doi:10.5061/dryad.32765 
   - Immunohistochemical typing of adenocarcinomas https://datadryad.org/stash/dataset/doi:10.5061/dryad.g8h71
   - Clinical, molecular, and spatial data in breast cancer https://datadryad.org/stash/dataset/doi:10.5061/dryad.828nn 
2. Identify three research questions to answer using tools applied this semester. Appropriate questions include performing data filtering/assessment/grouping followed by summary statistics/machine learning and assessing patterns using data visualization. Please note:
   - The data you select from the list above may not follow best practices in data organization. You may need to convert file formats of the data prior to analyzing. We recommend you assess (and document) things like column headers and encoding of missing data as a part of your analysis.
   - Some of these datasets are not particularly well-documented. The original manuscripts may provide additional context, but you will have the opportunity to describe the assumptions you made about the data and what could've been done to improve their reusability.
   - These data come from previously published research studies. You are not required to ask the same questions as the original publications; this assignment is deliberately open-ended to allow you freedom to select from the tools we've used this semester.
   - Your questions should require more than a minimal level of coding effort to assess (e.g., it is unacceptable to ask “What is the mean of [some column] in the dataset?”). However, you are also not required to apply advanced statistical testing in your analysis beyond what we have explicitly covered in class. The focus of this assignment is aligning code with data and interpreting conclusions, rather than performing rigorous tests. 
   - You should include at least two data visualizations in your project, and apply best practices in visualization design as described in the first part of our course.
   - An (oversimplified) example with questions/results: If you chose a dataset representing student enrollment in 200 different courses throughout ten years, your questions would be 1) Are all classes present across the entirety of the timeframe? (result is a yes or no, if no, include the number of classes that aren’t present), 2) What is the average enrollment in the largest 10 classes across ten years? (result is a table and line graph), 3) Does enrollment in each course vary with total enrollment across all classes? (result is a density plot with overlay of total enrollment)
3. Set up a project repository in GitHub. Your repository should: 
   - Represent appropriate practices for a project directory (subdirectories, file naming, etc) as described in the first few classes.
   - Not include large data files (>50 MB). You will not be able to push large data files to GitHub. We recommend use of a `.gitignore` file, storing large files in other locations outside your project directory, and use of smaller/filtered/reduced intermediate data files when appropriate. 
   - Track a reasonable version history of your project as it develops. In other words, you should not have only an initial commit and then upload of the final files (aim for at least two commits!).
4. Document your data, code, and other project components with a `README` file. This should follow best practices covered in the first part of the course, including (but not necessarily limited to):
   - Explanations of the directory structure and all included files.
   - Description of the data (with citation) and where it can be found online
   - If not readily apparent from your code, it may be useful to specify information about your environment (software versions, local vs. remote computing, etc).
5. Write code to answer your three research questions. Your code should include:
   - A markdown (`report_r.md` or `report_r.Rmd`) and ipython notebook (`report_python.ipynb`) serving as a final report that includes the following:
   - A written (markdown) section at the top of one of the reports titled “About the data” that describes any assumptions you made about the data and what would’ve improved your ability to reuse it.
   - A meaningful title and brief (markdown) introduction to each report.
   - Each research question clearly stated, associated code, results/conclusions/interpretations (which may include print statements, markdown text chunks, and data visualizations).
   - Complete code comments that describe the tasks being accomplished.
   - For each visualization, a justification for the type of visualization and your formatting choices.
   - A written (markdown formatted) section at the end of one report titled “Reproducibility” that comments on the ease of reproducibility of your analysis and the analysis in the original paper, which reflects on the concepts covered in the first few weeks of class.
   -  In addition to your report, you may (but are not required to) include additional files used for analysis (either as intermediate results, or scripts). Make sure they are documented in your README!
        
## Rubric

| **Criteria | Expert (20)  | Competent (16)       | Needs work (12)**
|---------|--------|------------------|--------
| **Content of code**      | Code includes both R and Python, is executable and fully commented, text answers formatted appropriately with markdown   | Code is missing one major or multiple minor components and/or comments, may not run to completion or have errors, markdown does not render appropriately    | Code is largely incomplete, missing comments, cannot run to completion or has errors, and markdown text not included
| **Project organization and documentation** | Project organized following best practices and documented in README, Git and GitHub use  | Project partially organized and/or does not follow best practices, README incomplete; Git/GitHub not fully implemented       | Project lacking basic organizational structure; README missing/incomplete; no useful Git history
| **Research questions and conclusions** | Three robust research questions clearly stated with results/conclusions, visualizations justified and follow design best practices  | Three research questions stated and partially aligned with associated code and results/conclusions, visualizations partially justified and/or do not follow design best practices       | Three research questions with code/results incomplete, visualizations lacking justification and/or do not follow design best practices
| **Content of written responses** | Title/introduction present, “About the data” describes assumptions and recommendations for improvement, “Reproducibility” comments on both original analysis and reuse in this project  | All required components present but missing detail and/or possess minor inaccuracies       | One or more required response missing, incomplete, and/or with multiple inaccuracies
