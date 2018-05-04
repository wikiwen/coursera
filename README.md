# Coursera

## Downloading all the assignments jupyter notebooks and files   
1 Go to the home of the coursera-notebook hub  
2 Create a new python notebook  
3 Execute !tar cvfz allfiles.tar.gz * in a cell  
4 Download the archive !  
参考：https://www.reddit.com/r/learnmachinelearning/comments/7er5ps/coursera_downloading_all_the_assignments_jupyter/

## Downloading all materials of the course, like videos,ppts,etc
### Install the script: coursera-dl
    pip install coursera-dl
### Running the script
Run the script to download the materials by providing your Coursera account credentials (e.g. email address and password or a ~/.netrc file), the class names, as well as any additional parameters:
    
    General:                     coursera-dl -u <user_name> -p <passport> <course_name>
    Multiple classes:            coursera-dl -u <user> -p <pass> <course_name1> <course_name2> <course_name3>
    Filter by section name:      coursera-dl -u <user> -p <pass> -sf "Chapter_Four" <course_name>
    Filter by lecture name:      coursera-dl -u <user> -p <pass> -lf "3.1_" <course_name>
    Download only ppt files:     coursera-dl -u <user> -p <pass> -f "ppt" <course_name>
    Download only mp4 files:     coursera-dl -u <user> -p <pass> -f "mp4" <course_name>
    Use a ~/.netrc file:         coursera-dl -n -- <course_name>
    Get the preview classes:     coursera-dl -n -b <course_name>
    Specify download path:       coursera-dl -n --path=<the path you want to save on> <course_name>
    Display help:                coursera-dl --help

    Maintain a list of classes in a dir:
    Initialize:              mkdir -p CURRENT/{class1,class2,..classN}
    Update:                  coursera-dl -n --path CURRENT `\ls CURRENT`
### Resuming downloads
    coursera-dl -u <user> -p <pass> --resume <course_name>
    
转载自：https://github.com/coursera-dl/coursera-dl
