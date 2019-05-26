# Workshop agenda

In this workshop, we're aiming to introduce you to a point cloud processing and visualisation workflow using open source toolkits.

We'll use the Point Data Abstraction Library (PDAL), Python, Entwine and the Potree WebGL-based viewer to interrogate point cloud data, perform some basic analyses, modify our points and visualise them in a web browser.

On the way we'll learn how to use PDAL's pipeline system, as well as providing parameters to processing pipelines via command line input. We'll drive PDAL using a combination of docker command line invocations, and exploiting it as a Python library.

Finally, we'll use Entwine to create a visualisation-ready version of our data, and explore it in the Potree viewer.

In this workshop we will learn by doing - it'll be a bit of a magical mystery tour in that many concepts will be shown, then discussed.

## Getting started

Workshop is based on OSGeoLive12 just because is the generic platform used for SIGLibre worksops, but most of the this workshop will run inside a Anaconda/Conda or Docker environment. The virtualmachine of the workshop is prepared with Anaconda environment and some docker images installed.

VirtualBox VM can be downloaded from: 

https://mega.nz/#!RQREgYyY with key `4neDT5Gv1dwjzrV_4KT9fLp0e3FuKBy9I5fhIk5pQJA`

VM will be available for a month after the workshop and then removed!

### Conda setup

Most of the workshop will be executed in Terminal where we will activate the conda environonment and related workshop virtual environment.
The reason to run all warkshop in virtual env is because I need QGIS installed in Conda environment to allow QGIS using the same PAL and python interpreter.
Follow these steps to activate the workshop environment.

`user@osgeolive:~$ cd`
`user@osgeolive:~$ source ./anaconda3/bin/activate`
`(base) user@osgeolive:~$ conda activate f4g-pdal-workshop`
`(f4g-pdal-workshop) user@osgeolive:~$`

### Clone workshop material

Workshop material is already cloned at:

`/home/user/Workshop/f4g-oceania-pdal`

If you need to replicate at home, open a command line window (if you can use bash, great!) and do:

`git pull https://github.com/luipir/f4g-oceania-pdal.git`

that is a fork of `https://github.com/adamsteer/f4g-oceania-pdal.git` with the agreement of the author.

sample datasets is at:

`/home/user/Workshop/sample-data`

All of our exercises today are run from there.

## Questions and feedback

Feel free to ask questions anytime. Be aware you may be asked to wait for an answer...

Please give feedback! Use the post-it notes to provide anonymous feedback. We'll use software carpentry style, 1 up, 1 down feedback on sticky notes. At break time stick them to the wall, and I'll read them. If anything can be improved for the second session, we'll try to do it. A feedback session will be held at the end. Don't be shy here - the longer you wait to provide input the harder your task will be!

## Running order

### Session 1 [1:30 - 3:10, 100 minutes]
[10 min] Introducing instructors and helpers, housekeeping.

#### Introductions
[10 min] Who are you? why are you here? what do you want to achieve?

#### Preamble
[20 min] Point clouds, why PDAL, what are some alternatives, room for discussion

#### Starting out with PDAL
[30 min] Thinking in PDAL, PDAL on the command line, using conda or docker - to query metadata and points; Introduction to processing pipelines.

#### Processing data with PDAL
[30 min] Using a pipeline to find ground points, and reduce noise

### Break [20 min]

### Session 2 [3:30 - 5:00 pm, 90 minutes]

#### Python and PDAL
[30 min] Using python code in PDAL, using PDAL as a python library with Jupyter notebooks for exploratory analysis

#### Entwine
[20 min] Introduction to Entwine; creating an entwine EPT index; Setting up and viewing entwine datasets on a local web server


#### Future visions and discussion

[10 min] Where I see this going, and where do **you** see this going?

#### Formal feedback discussion
[10 min] Wrap up; one up, one down feedback

[next - pointclouds](0-pointclouds.md)
