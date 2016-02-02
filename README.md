# wercker-step-releasequeue-deploy
A Wercker step to upload deb/rpm packages to ReleaseQueue Server
Example usage:
```
    - releasequeue/releasequeue-deploy@0.0.10:
        distribution: "trusty"
        component: "extras"
        username: "admin"
        apikey: "<my_api_key>"
        package: "package.deb"

```
Parameters:

* username: ReleaseQueue username
* apikey: ReleaseQueue api key
* package: path to package you want to upload
* distribution: distribution associated with package(needs to be present in your ReleaseQueue config)
* component: component associated with package(needs to be present in your ReleaseQueue config)
