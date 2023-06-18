# grpEHR training

Tips for using Git and GitHub aimed at new users of the [OpenSAFELY](https://www.opensafely.org/) system and some best practice tips.

Rendered at <https://grpehr.github.io/training/>

To build/render the html output

* Install Quarto from [here](https://quarto.org/docs/get-started/) or on macOS install from Homebrew with
  ```
  brew install --cask quarto
  ```
* Open the RStudio project in RStudio by double-clicking the *training.Rproj* file
* In RStudio open the *Build* pane and click the *Build Website* button
* or, run in R
  ```r
  # install.packages('quarto')
  quarto::quarto_render()
  ```

  Or in a terminal, run
  ```bash
  quarto render
  ```

* Commit the changes to both the source *.qmd* files and *.html* output in the *docs* directory into the repo.

* When editing the project, you can preview the html output with
  ```r
  quarto::quarto_preview()
  ```
  which is stopped with
  ```r
  quarto::quarto_preview_stop()
  ```
  or in a terminal, run
  ```bash
  quarto preview
  ```
  which is stopped by pressing <kbd>Ctrl</kbd>+<kbd>C</kbd> in the same terminal window
