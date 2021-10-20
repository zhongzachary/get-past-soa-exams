# Get Past SOA Exams

Have you got tired of clicking all the links in SOA's website to download all the past exams? You come to the right place.

This `R` script will scrap all the available files in [SOA's website](https://www.soa.org/education/exam-req/syllabus-study-materials/edu-multiple-choice-exam), and download it for you.

All you need is `R` ([download here](https://cloud.r-project.org)) and `RStudio` ([download here](https://www.rstudio.com/products/rstudio/download/)). 
You might also need some basic knowledge on how to run a `R Markdown` in `RStudio`.

## Directions
- Open `get_past_exams.Rmd` script in `RStudio`. It will install all the required packages for you.
- Run all the cells except the last 2 cells.
- In the second-to-last cell, change the exam name to the exam you want to download.
  - The provided code is trying to download all files for Exam PA. You can change it to other exams.
    ```{R}
    # change Exam PA to your exam in the cell
    download.files.data <- files.data %>% filter(exam == 'Exam PA')  
    ```
  - You can refer to the previous cells in the script on what are the available exams.
- Run the last cell to download the exam. 
  - All files will be downloaded in the same location as this `R` project.
  - There will be a folder for each exam sitting.
  - It should work for different operating systems.
