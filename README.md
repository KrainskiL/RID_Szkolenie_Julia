# Julia Training - RID
The repository contains materials for the training **Introduction to Data Science and Machine Learning with Julia** conducted as part of the SGH Regional Excellence Initiative.

## Agenda
1. Introduction to Julia
2. Virtual Environment and Package Management
3. Basic Data Types
4. Overview of Matrix and Vector Operations
5. Vectorization of Code (dot operator)
6. Working with Data Frames (DataFrames.jl, CSV.jl)
7. Data Visualization with Plots.jl Library
8. Generating Plots for Scientific Papers with PGFPlotsX.jl
9. Introduction to Machine Learning with Julia – MLJ.jl
10. Notes on Integration with Other Programming Languages ​​– Python and R

## Meetings
* 14.03.2025 14:00-16:30 MS Teams
* 21.03.2025 14:00-16:30 MS Teams

## Environment setup

1. Install [Julia](https://julialang.org/downloads/). It is recommended to install without administrator privileges (installation for active user). During the training we will use version **v1.11.4**.
2. Download materials:
    * Download the archive via the green button `Code` -> `Download zip` and unpack it in an easily accessible location OR
    * Clone the repository using the command `git clone https://github.com/KrainskiL/RID_Szkolenie_Julia` in the terminal
3. Open terminal and make sure the working path is in the root folder of the downloaded repository.
```bash
cd RID_Szkolenie_Julia # or cd RID_Szkolenie_Julia-main
```
4. Start Julia with the `julia` command. If you get an error about the application not being installed, check if Julia is in your [PATH environment variable](https://julialang.org/downloads/platform/).
5. Once you have launched Julia's REPL, type the following commands:
```julia
using Pkg
pkg"activate ." # activating virtual environment
pkg"instantiate"   # installation of required packages
```
6. Install the notebook environment using IJulia (commands in Julia REPL):
```julia
using IJulia
notebook(dir=".")
# Accept with Y
```
If Jupyter was already installed on the machine, step 6 can be skipped - after step 5, the Julia kernel should be available in the Jupyter interface.

## Latex

To properly run `3_Plots_Latex.ipynb` notebook, you'll need Latex distribution installed e.g. [TexLive](https://www.tug.org/texlive/) or [MikTex](https://miktex.org/download). 


## Visual Studio Code

An alternative way to work with training materials is the IDE [Visual Studio Code](https://code.visualstudio.com/). To work with Julia, it is recommended to install the [official plugin](https://github.com/julia-vscode/julia-vscode). VS Code provides a dedicated notebook editor and many features useful in creating and testing source code. ⚠️ A small part of the notebook commands may not work correctly in the VS Code environment.

## Additional materials

[Julia Academy](https://juliaacademy.com/)

[Julia Language Manual](https://docs.julialang.org/en/v1/)

[Julia for Data Analysis](https://www.manning.com/books/julia-for-data-analysis)
