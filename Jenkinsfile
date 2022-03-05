This file is for Jenkins groovy script
We will install

#!/bin/bash
folders='images music videos'
ext_images="*.jpg *.png"
ext_music="*.mp3 *.flac"
ext_videos="*.avi *.mov"

for folder in $folders
do
        if [ $folder == 'images' ]
        then
                mkdir -p $folder
                mv $ext_images $folder 2>/dev/null

        elif [ $folder == 'music' ]
        then
                mkdir -p $folder
                mv $ext_music $folder 2>/dev/null

        elif [ $folder == 'videos' ]
        then
                mkdir -p $folder
                mv $ext_videos $folder 2>/dev/null

        else
        find . -name "*.log" -type f -delete
                echo "$(tput setaf 3)Unable to create folder..$(tput sgr0)"
        fi

done

echo "$(tput setaf 2)Directory organized successfully..$(tput sgr0)"
