 # Create new file in the READMe fine



#!/bin/bash

        #AUTHER: Kenneth
        #DATE: 19-11-22
#................ INSTALLATION OF PACKAGES ........................


CURRENT_OS=$(hostnamectl | grep -i Operating | awk -F " " '{print $3}')

echo ${CURRENT_OS}

sleep 4

if [ ${CURRENT_OS} == Ubuntu ]
then
        echo 'success, You are using CentOS System'
elif [ ${CURRENT_OS} == Centos ]
then
        echo 'Success, You are using CentOS system'
else 
        echo 'hmmmm, You have to use either Ubuntu or CentOS for this script'
fi

echo 'script worked'
