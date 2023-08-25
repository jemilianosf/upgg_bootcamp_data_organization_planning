# UPGG Bootcamp Data And Project Organization Notes
2023-08-25


## Setup

- Create a new directory 
```
mkdir 20230825_upgg_bootcamp_data_organization
cd 20230825_upgg_bootcamp_data_organization/
```

- Download data
```
wget https://reproducible-science-curriculum.github.io/organization-RR-Jupyter/data/gapminderDataFiveYear_superDirty.xlsx
wget https://reproducible-science-curriculum.github.io/organization-RR-Jupyter/data/gapminderDataFiveYear_superDirty.txt
```

## Intro

- Inspect table and ask questions
```
head gapminderDataFiveYear_superDirty.txt
tail gapminderDataFiveYear_superDirty.txt
```

## Project Structure

### How to structure project folders and name files

- Two main strategies to make analysis easier to follow: organization and documentation
- Go through slides
- After conclusions ask folks to put github link to notes

### Putting it to practice
- Do exercise / ask quesitons

- After tips and tricks section: create data directory and raw data subdirectory
```
mkdir data
mkdir data/raw
```

- Move raw data to raw data directory 
```
mv gapminderDataFiveYear_superDirty.* data/raw/
cd data/raw/
```

- Make text files read only
```
chmod 444 gapminderDataFiveYear_superDirty.txt
chmod 444 gapminderDataFiveYear_superDirty.xlsx
```

- Ask to Try to remove or edit
```
nano gapminderDataFiveYear_superDirty.txt
rm gapminderDataFiveYear_superDirty.txt
```

### Record keeping
- The second approach is record keeping and metatadata 


## Metadata

### Why READMEs

### Adding a Top Level README

- Go back to main directory
```
cd ../../
```

- Create readme
```
nano README.txt
```

### Adding a README in a Subdirectory

- Go to raw data and create readme
```
nano data/raw/README.txt
```

### Keeping the READMEs up-to-date

### Self-documenting Projects

- Project readme example



## Modifying Data

### Activity: Sanity-check the data

### Should we fix any of the problems we see in this file? Why or why not?

Make cleaned directory
```
cd data
mkdir cleaned
```

Create a copy of data
```
cp raw/gapminderDataFiveYear_superDirty.xlsx cleaned/.
cd cleaned/
chmod 755 gapminderDataFiveYear_superDirty.xlsx
```

Modify data (remove duplicated row)

```
open gapminderDataFiveYear_superDirty.xlsx
```

Add data modifications by hand to readme
```
nano README.txt
```

### Pitfalls of manually cleaning data

## Concluding thoughts

### Completing our project directory
Go back to main directory 
```
cd ..
```

Create rest of directory
```
mkdir output
mkdir code
```

Take a final look
```
ls
```

## Examples

- Examples from rotation

- Example template
https://github.com/jemilianosf/template_analysis

- Make a github repository template:
https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-template-repository

