# MathSuccess Dataset Analysis

## Overview
This project analyzes the **MathSuccess dataset**, which contains data on student performance, including their scores from various entrance exams and their final course success. The goal is to compare multiple machine learning algorithms to determine which model best predicts student success.

## Table of Contents
- [Dataset Description](#dataset-description)
- [Preprocessing Steps](#preprocessing-steps)
- [Algorithms Used](#algorithms-used)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Dataset Description
The MathSuccess dataset consists of approximately 2600 rows with the following columns:
- **Student**: Identifier for each student.
- **Gender**: Gender of the student.
- **PSATM**: Score from the PSAT exam.
- **SATM**: Score from the SAT exam.
- **ACTM**: Score from the ACT exam.
- **Rank**: Academic rank of the student.
- **Size**: Size of the school.
- **GPAadj**: Adjusted GPA.
- **PlcmtScore**: Placement score.
- **Recommends**: Recommendations received.
- **Course**: Course taken by the student.
- **Grade**: Grade received in the course.
- **RecTaken**: Recommendations taken into account.
- **TooHigh/TooLow**: Indicators for admission test scores.
- **CourseSuccess**: Outcome variable indicating whether the student passed or failed.

## Preprocessing Steps
1. Removed rows with missing values in the CourseSuccess column.
2. Replaced missing values in other columns with zero.
3. Converted categorical variables (Recommends, Grade, CourseSuccess) into factors.

## Algorithms Used
The following machine learning algorithms were implemented:
1. **CART (Classification and Regression Trees)**
2. **RPart (Recursive Partitioning)**
3. **Support Vector Machine (SVM)**
4. **Random Forest**
5. **Neural Network**

Each algorithm was chosen based on its strengths in handling classification tasks and its ability to provide insights into student performance.

## Results
The performance metrics for each algorithm are summarized below:

| Algorithm          | Accuracy | Precision | Recall | F1 Score | Error Rate |
|--------------------|----------|-----------|--------|----------|------------|
| C_Tree             | 0.9953   | 1.0000    | 0.9931 | 0.9965   | 0.0047     |
| R_Part             | 1.0000   | 1.0000    | 1.0000 | 1.0000   | 0.0000     |
| SVM                | 0.9812   | 1.0000    | 0.9730 | 0.9863   | 0.0188     |
| Random Forest      | 0.9930   | 1.0000    | 0.9897 | 0.9948   | 0.0070     |
| Neural Network     | 0.9953   | 1.0000    | 0.9931 | 0.9965   | 0.0047     |

## Installation
To run this project, ensure you have R and RStudio installed on your machine, along with the following libraries:
```r
install.packages(c("rpart", "party", "e1071", "randomForest", "nnet", "caTools"))
```

## Usage
Clone this repository and run the code in RStudio to replicate the analysis:
```bash
git clone https://github.com/yourusername/MathSuccessAnalysis.git
cd MathSuccessAnalysis
```

Open `analysis.R` in RStudio and execute the code to see results.

## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adjust any sections according to your preferences or add any additional information that may be relevant to your project!

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/23864058/2f3d7bfb-4067-492b-aa36-82edb5a9f5f2/Screenshot-2024-11-05-at-8.16.54-PM.pdf
