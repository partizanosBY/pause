# pause

pause image for windows 2019 1903

Kubernetes 1.17.2 out of the box does not support Windows 2019 1903.
To launch docker containers in the windows version of kubernetes, you need to replace the pause image: 

docker build . -t kubeletwin/pause -t mcr.microsoft.com/k8s/core/pause:1.2.0
