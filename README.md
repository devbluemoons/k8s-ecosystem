# k8s-ecosystem
kubernetes centerd projects by CNCF
  
## <img src="https://landscape.cncf.io/logos/helm.svg" width="111" />
The package manager for Kubernetes

###### install / uninstall
```sh
# uninstall (Debian/Ubuntu)
$ which helm
/some/path/to/helm
$ rm -rf /some/path/to/helm

# install (Debian/Ubuntu)
curl https://baltocdn.com/helm/signing.asc | sudo apt-key add -
sudo apt-get install apt-transport-https --yes
echo "deb https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
sudo apt-get update
sudo apt-get install helm
```
###### common
```sh
# check version
helm version

# add repository
helm repo add [NAME] [URL]

# update repostiroy
helm repo update

# get repository list
hlem repo list

# search chart version
helm search repo [CHART]

# install chart
helm install [RELEASE_NAME] [CHART] [flags]

# install chart directory `An unpacked chart directory`
helm install [CHART_DIREACTORY] [flags]

# uninstall chart
helm uninstall [RELEASE_NAME] [flags]

# get chart list
helm list [flags]

# upgrade chart
helm upgrade [RELEASE_NAME] [CHART] [flags]

# create chart
helm create [CHART]

helm dependency update [CHART_DIREACTORY]

# get chart config info
helm get notes [CHART-NAME] [NAMESPACE]
```
