This program allows you to get the Todoist task completion history, per project.

# Getting started

After cloning the repo:

    go get github.com/bitly/go-simplejson
    go get github.com/fatih/color
    go build
    
From https://todoist.com/app under Settings > Integrations get your token. To get the tasks completed last week:

    ./todoistcomplete -SinceDate=`date -dlast-monday +%m/%d/%Y` \
        -UntilDate=`date -dlast-sunday +%m/%d/%Y` \
        -Token=qwertyuiopasdfghjklzxcvbnm
