<img src="images/GEMS Informatics Learning.png" width=600 alt="GEMS Learning Logo" title="GEMS Learning" />

# X003.0 An Introduction to Spatial Data Analysis in R

This course is designed for those who are interested in explicitly accounting for location in their analyses. Through this 3-week introductory course, you will learn how to work with spatial data in R, starting from importing different spatial datasets and creating simple maps, to conducting basic geocomputation on vector and raster data. In each 2.5 hour lecture, you will have the opportunity to immediately practice your new skills via hands-on exercises focused on agri-food applications. 

- Week 1: Introduction to spatial data and mapping in R
- Week 2: Basic geocomputation with vector data in R
- Week 3: Basic geocomputation with raster data in R 

The course will be delivered via a Jupyter Notebook hosted on the GEMS Informatics Platform. You do not need to have R or RStudio installed on your machine to participate.

## Prerequisites: 
- Access to the internet
- A [GEMS Platform](https://gems.agroinformatics.org/webui/#) user account
- Introductory knowledge of R & RStudio  

## Initial Setup
1. Login to GEMS Platform at https://gems.agroinformatics.org/
    - GEMS Platform uses Globus to authenticate your account, so if your institution is already linked to Globus (for example, University of Minnesota and many other universities), you can search and select your institution from the list and use your institutional account to log into GEMS Platform. Alternatively, you can log in using Google or ORCID iD, or create  your own Globus account to log in.   
    
2. Once logged in, click `Analyze > RStudio` from the homepage (top right corner). If you do not have an `Analyze` option next to `Data Products` and `My Workspace` please let your TA know immediately. They will need to assign you permissions using their administrator account. 

3. Install packages needed for course. If you have any issues please let your TA know immediately. 
    ```shell
    packages_to_install <- c("tmap", "spData")
    
    for ( package in packages_to_install ) {
        if (!require(package, character.only=T, quietly=T, warn.conflicts=F)) {
            install.packages(package)
        }
    }
    ```

4. While your packages are installing, navigate to the `Terminal` tab in your Console Window

5. If the directories `classes\GEMSX003` were not created before, create directories for this class in the bash terminal using the following four commands  
    ```shell
    mkdir classes  
    cd classes  
    mkdir GEMSX003  
    cd GEMSX003
    ```  
    If these directories already exist, use the following commands to change to this directory
    ```shell
    cd classes
    cd GEMSX003
    ```
    
    
## Week 1 Lecture: Introduction to spatial data and mapping in R
1. Navigate to your `GEMSX003` directory using the following commands:
    ```shell
    cd classes
    cd GEMSX003
    ```
2. Clone the git repository for this week's lecture  
    ```shell
    git clone https://github.com/abjoglekar/GEMS-X003-Geospatial-Analysis-R-Intro.git
    ```
3. From your files, navigate to your `GEMS-X003-Geospatial-Analysis-R-Intro > scripts` directory and open the `02_GEMSX003.0_Points.Rmd` R Markdown file to follow along for the first hands on component. 

