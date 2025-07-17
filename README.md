# Rao tutorial

[Rao](https://www.lotas.ai/) is a fork of RStudio with a fully integrated AI assistant that can read, write, and edit code; search for context; run code and commands; and view and interpret outputs. Its source code is [available here](https://github.com/lotas-ai/rao). If you have questions or bug reports, please direct them to the [Lotas Forum](https://community.lotas.ai/). 

*The following is a tutorial prepared for the Curtis Huttenhower lab meeting on July 18, 2025.*

## 1. Installing R and Rao

[R](https://www.r-project.org/) is a programming language specializing in statistical computing and graphics. You can use R just the same as any other programming languages, but it is most useful for statistical analyses, with well-established packages for common tasks such as [linear modeling](https://cran.r-project.org/web/packages/lme4/index.html), ['omic data analysis](https://bioconductor.org/), [machine learning](http://topepo.github.io/caret/index.html), and [visualization](https://ggplot2.tidyverse.org/).

#### Installing R for the first time

You can download and install the free R software environment [here](https://cloud.r-project.org/). Note that you should download the latest release (and no older than version 4.0) - this will ensure the R version you have is compatible with Rao.

#### Installing Rao

1. Go to the [Rao download page](https://www.lotas.ai/download) and download Rao for your machine.
2. Go to the [Account page](https://www.lotas.ai/account), make an account if necessary, and copy your API key.
3. Open the app, click on the AI pane in the top right (or enable it if necessary, see ["Opening the AI Pane"](https://www.lotas.ai/download)), click on the setting gear in the top left of the pane, and paste in your API key.

Once you've done this, you should see the following section (you might need to click the gear to refresh):
<img src="https://github.com/lotas-ai/hutlab-demo/blob/713934d127340dd058dcb777983997b9c00720e4/media/images/rao-profile.jpg" style="width:75%;">

#### Setting a working directory

Rao works by indexing your current directory so that it can find files, functions, code blocks, etc. more quickly. Therefore, it's helpful to set your working directory to a narrow directory where you'll perform your analysis. You can check your current working directory with `getwd()` and then create a folder for this demo like:

```
dir.create('tutorial')
```

Then, use the "Browse..." button of the "Working Directory" section or use `setwd()` to set your working directory to the folder you create.
