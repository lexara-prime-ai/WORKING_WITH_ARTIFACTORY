# Working with Artifactory
* Downloading a **pre-built** wheel file
```powershell
curl -sSf -H "X-JFrog-Art-Api:<YOUR_ARTIFACTORY_TOKEN>" \
          -O 'https://your-organization.jfrog.io/artifactory/pypi-internal/my-python-library/0.1.0/my-python-library-0.1.0-py3-none-any.whl'
```

* Using **wget**
```powershell
wget --header="X-JFrog-Art-Api:<YOUR_ARTIFACTORY_TOKEN>" 'https://your-organization.jfrog.io/artifactory/pypi-internal/my-python-library/0.1.0/my-python-library-0.1.0-py3-none-any.whl'
```

* Using **Github worflows**
```powershell
wget --header="X-JFrog-Art-Api:{{ secrets.ARTIFACTORY_TOKEN }}" 'https://your-organization.jfrog.io/artifactory/pypi-internal/my-python-library/0.1.0/my-python-library-0.1.0-py3-none-any.whl'
```



