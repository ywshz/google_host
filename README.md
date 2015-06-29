#!/bin/bash
WORK_FOLDER=/Users/ywszjut/Desktop

curl https://raw.githubusercontent.com/racaljk/hosts/master/hosts > $WORK_FOLDER/google.hosts

cat $WORK_FOLDER/host.bak > $WORK_FOLDER/hosts
cat $WORK_FOLDER/google.hosts >> $WORK_FOLDER/hosts

cat $WORK_FOLDER/hosts > /etc/hosts

