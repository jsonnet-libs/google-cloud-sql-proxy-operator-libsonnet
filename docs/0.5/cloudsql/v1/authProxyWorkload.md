---
permalink: /0.5/cloudsql/v1/authProxyWorkload/
---

# cloudsql.v1.authProxyWorkload

"AuthProxyWorkload declares how a Cloud SQL Proxy container should be applied to a matching set of workloads, and shows the status of those proxy containers."

## Index

* [`fn new(name)`](#fn-new)
* [`obj metadata`](#obj-metadata)
  * [`fn withAnnotations(annotations)`](#fn-metadatawithannotations)
  * [`fn withAnnotationsMixin(annotations)`](#fn-metadatawithannotationsmixin)
  * [`fn withClusterName(clusterName)`](#fn-metadatawithclustername)
  * [`fn withCreationTimestamp(creationTimestamp)`](#fn-metadatawithcreationtimestamp)
  * [`fn withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)`](#fn-metadatawithdeletiongraceperiodseconds)
  * [`fn withDeletionTimestamp(deletionTimestamp)`](#fn-metadatawithdeletiontimestamp)
  * [`fn withFinalizers(finalizers)`](#fn-metadatawithfinalizers)
  * [`fn withFinalizersMixin(finalizers)`](#fn-metadatawithfinalizersmixin)
  * [`fn withGenerateName(generateName)`](#fn-metadatawithgeneratename)
  * [`fn withGeneration(generation)`](#fn-metadatawithgeneration)
  * [`fn withLabels(labels)`](#fn-metadatawithlabels)
  * [`fn withLabelsMixin(labels)`](#fn-metadatawithlabelsmixin)
  * [`fn withName(name)`](#fn-metadatawithname)
  * [`fn withNamespace(namespace)`](#fn-metadatawithnamespace)
  * [`fn withOwnerReferences(ownerReferences)`](#fn-metadatawithownerreferences)
  * [`fn withOwnerReferencesMixin(ownerReferences)`](#fn-metadatawithownerreferencesmixin)
  * [`fn withResourceVersion(resourceVersion)`](#fn-metadatawithresourceversion)
  * [`fn withSelfLink(selfLink)`](#fn-metadatawithselflink)
  * [`fn withUid(uid)`](#fn-metadatawithuid)
* [`obj spec`](#obj-spec)
  * [`fn withInstances(instances)`](#fn-specwithinstances)
  * [`fn withInstancesMixin(instances)`](#fn-specwithinstancesmixin)
  * [`obj spec.authProxyContainer`](#obj-specauthproxycontainer)
    * [`fn withImage(image)`](#fn-specauthproxycontainerwithimage)
    * [`fn withMaxConnections(maxConnections)`](#fn-specauthproxycontainerwithmaxconnections)
    * [`fn withMaxSigtermDelay(maxSigtermDelay)`](#fn-specauthproxycontainerwithmaxsigtermdelay)
    * [`fn withRolloutStrategy(rolloutStrategy)`](#fn-specauthproxycontainerwithrolloutstrategy)
    * [`fn withSqlAdminAPIEndpoint(sqlAdminAPIEndpoint)`](#fn-specauthproxycontainerwithsqladminapiendpoint)
    * [`obj spec.authProxyContainer.adminServer`](#obj-specauthproxycontaineradminserver)
      * [`fn withEnableAPIs(enableAPIs)`](#fn-specauthproxycontaineradminserverwithenableapis)
      * [`fn withEnableAPIsMixin(enableAPIs)`](#fn-specauthproxycontaineradminserverwithenableapismixin)
      * [`fn withPort(port)`](#fn-specauthproxycontaineradminserverwithport)
    * [`obj spec.authProxyContainer.container`](#obj-specauthproxycontainercontainer)
      * [`fn withArgs(args)`](#fn-specauthproxycontainercontainerwithargs)
      * [`fn withArgsMixin(args)`](#fn-specauthproxycontainercontainerwithargsmixin)
      * [`fn withCommand(command)`](#fn-specauthproxycontainercontainerwithcommand)
      * [`fn withCommandMixin(command)`](#fn-specauthproxycontainercontainerwithcommandmixin)
      * [`fn withEnv(env)`](#fn-specauthproxycontainercontainerwithenv)
      * [`fn withEnvFrom(envFrom)`](#fn-specauthproxycontainercontainerwithenvfrom)
      * [`fn withEnvFromMixin(envFrom)`](#fn-specauthproxycontainercontainerwithenvfrommixin)
      * [`fn withEnvMixin(env)`](#fn-specauthproxycontainercontainerwithenvmixin)
      * [`fn withImage(image)`](#fn-specauthproxycontainercontainerwithimage)
      * [`fn withImagePullPolicy(imagePullPolicy)`](#fn-specauthproxycontainercontainerwithimagepullpolicy)
      * [`fn withName(name)`](#fn-specauthproxycontainercontainerwithname)
      * [`fn withPorts(ports)`](#fn-specauthproxycontainercontainerwithports)
      * [`fn withPortsMixin(ports)`](#fn-specauthproxycontainercontainerwithportsmixin)
      * [`fn withStdin(stdin)`](#fn-specauthproxycontainercontainerwithstdin)
      * [`fn withStdinOnce(stdinOnce)`](#fn-specauthproxycontainercontainerwithstdinonce)
      * [`fn withTerminationMessagePath(terminationMessagePath)`](#fn-specauthproxycontainercontainerwithterminationmessagepath)
      * [`fn withTerminationMessagePolicy(terminationMessagePolicy)`](#fn-specauthproxycontainercontainerwithterminationmessagepolicy)
      * [`fn withTty(tty)`](#fn-specauthproxycontainercontainerwithtty)
      * [`fn withVolumeDevices(volumeDevices)`](#fn-specauthproxycontainercontainerwithvolumedevices)
      * [`fn withVolumeDevicesMixin(volumeDevices)`](#fn-specauthproxycontainercontainerwithvolumedevicesmixin)
      * [`fn withVolumeMounts(volumeMounts)`](#fn-specauthproxycontainercontainerwithvolumemounts)
      * [`fn withVolumeMountsMixin(volumeMounts)`](#fn-specauthproxycontainercontainerwithvolumemountsmixin)
      * [`fn withWorkingDir(workingDir)`](#fn-specauthproxycontainercontainerwithworkingdir)
      * [`obj spec.authProxyContainer.container.env`](#obj-specauthproxycontainercontainerenv)
        * [`fn withName(name)`](#fn-specauthproxycontainercontainerenvwithname)
        * [`fn withValue(value)`](#fn-specauthproxycontainercontainerenvwithvalue)
        * [`obj spec.authProxyContainer.container.env.valueFrom`](#obj-specauthproxycontainercontainerenvvaluefrom)
          * [`obj spec.authProxyContainer.container.env.valueFrom.configMapKeyRef`](#obj-specauthproxycontainercontainerenvvaluefromconfigmapkeyref)
            * [`fn withKey(key)`](#fn-specauthproxycontainercontainerenvvaluefromconfigmapkeyrefwithkey)
            * [`fn withName(name)`](#fn-specauthproxycontainercontainerenvvaluefromconfigmapkeyrefwithname)
            * [`fn withOptional(optional)`](#fn-specauthproxycontainercontainerenvvaluefromconfigmapkeyrefwithoptional)
          * [`obj spec.authProxyContainer.container.env.valueFrom.fieldRef`](#obj-specauthproxycontainercontainerenvvaluefromfieldref)
            * [`fn withApiVersion(apiVersion)`](#fn-specauthproxycontainercontainerenvvaluefromfieldrefwithapiversion)
            * [`fn withFieldPath(fieldPath)`](#fn-specauthproxycontainercontainerenvvaluefromfieldrefwithfieldpath)
          * [`obj spec.authProxyContainer.container.env.valueFrom.resourceFieldRef`](#obj-specauthproxycontainercontainerenvvaluefromresourcefieldref)
            * [`fn withContainerName(containerName)`](#fn-specauthproxycontainercontainerenvvaluefromresourcefieldrefwithcontainername)
            * [`fn withDivisor(divisor)`](#fn-specauthproxycontainercontainerenvvaluefromresourcefieldrefwithdivisor)
            * [`fn withResource(resource)`](#fn-specauthproxycontainercontainerenvvaluefromresourcefieldrefwithresource)
          * [`obj spec.authProxyContainer.container.env.valueFrom.secretKeyRef`](#obj-specauthproxycontainercontainerenvvaluefromsecretkeyref)
            * [`fn withKey(key)`](#fn-specauthproxycontainercontainerenvvaluefromsecretkeyrefwithkey)
            * [`fn withName(name)`](#fn-specauthproxycontainercontainerenvvaluefromsecretkeyrefwithname)
            * [`fn withOptional(optional)`](#fn-specauthproxycontainercontainerenvvaluefromsecretkeyrefwithoptional)
      * [`obj spec.authProxyContainer.container.envFrom`](#obj-specauthproxycontainercontainerenvfrom)
        * [`fn withPrefix(prefix)`](#fn-specauthproxycontainercontainerenvfromwithprefix)
        * [`obj spec.authProxyContainer.container.envFrom.configMapRef`](#obj-specauthproxycontainercontainerenvfromconfigmapref)
          * [`fn withName(name)`](#fn-specauthproxycontainercontainerenvfromconfigmaprefwithname)
          * [`fn withOptional(optional)`](#fn-specauthproxycontainercontainerenvfromconfigmaprefwithoptional)
        * [`obj spec.authProxyContainer.container.envFrom.secretRef`](#obj-specauthproxycontainercontainerenvfromsecretref)
          * [`fn withName(name)`](#fn-specauthproxycontainercontainerenvfromsecretrefwithname)
          * [`fn withOptional(optional)`](#fn-specauthproxycontainercontainerenvfromsecretrefwithoptional)
      * [`obj spec.authProxyContainer.container.lifecycle`](#obj-specauthproxycontainercontainerlifecycle)
        * [`obj spec.authProxyContainer.container.lifecycle.postStart`](#obj-specauthproxycontainercontainerlifecyclepoststart)
          * [`obj spec.authProxyContainer.container.lifecycle.postStart.exec`](#obj-specauthproxycontainercontainerlifecyclepoststartexec)
            * [`fn withCommand(command)`](#fn-specauthproxycontainercontainerlifecyclepoststartexecwithcommand)
            * [`fn withCommandMixin(command)`](#fn-specauthproxycontainercontainerlifecyclepoststartexecwithcommandmixin)
          * [`obj spec.authProxyContainer.container.lifecycle.postStart.httpGet`](#obj-specauthproxycontainercontainerlifecyclepoststarthttpget)
            * [`fn withHost(host)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgetwithhost)
            * [`fn withHttpHeaders(httpHeaders)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgetwithhttpheaders)
            * [`fn withHttpHeadersMixin(httpHeaders)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgetwithhttpheadersmixin)
            * [`fn withPath(path)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgetwithpath)
            * [`fn withPort(port)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgetwithport)
            * [`fn withScheme(scheme)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgetwithscheme)
            * [`obj spec.authProxyContainer.container.lifecycle.postStart.httpGet.httpHeaders`](#obj-specauthproxycontainercontainerlifecyclepoststarthttpgethttpheaders)
              * [`fn withName(name)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgethttpheaderswithname)
              * [`fn withValue(value)`](#fn-specauthproxycontainercontainerlifecyclepoststarthttpgethttpheaderswithvalue)
          * [`obj spec.authProxyContainer.container.lifecycle.postStart.tcpSocket`](#obj-specauthproxycontainercontainerlifecyclepoststarttcpsocket)
            * [`fn withHost(host)`](#fn-specauthproxycontainercontainerlifecyclepoststarttcpsocketwithhost)
            * [`fn withPort(port)`](#fn-specauthproxycontainercontainerlifecyclepoststarttcpsocketwithport)
        * [`obj spec.authProxyContainer.container.lifecycle.preStop`](#obj-specauthproxycontainercontainerlifecycleprestop)
          * [`obj spec.authProxyContainer.container.lifecycle.preStop.exec`](#obj-specauthproxycontainercontainerlifecycleprestopexec)
            * [`fn withCommand(command)`](#fn-specauthproxycontainercontainerlifecycleprestopexecwithcommand)
            * [`fn withCommandMixin(command)`](#fn-specauthproxycontainercontainerlifecycleprestopexecwithcommandmixin)
          * [`obj spec.authProxyContainer.container.lifecycle.preStop.httpGet`](#obj-specauthproxycontainercontainerlifecycleprestophttpget)
            * [`fn withHost(host)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgetwithhost)
            * [`fn withHttpHeaders(httpHeaders)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgetwithhttpheaders)
            * [`fn withHttpHeadersMixin(httpHeaders)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgetwithhttpheadersmixin)
            * [`fn withPath(path)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgetwithpath)
            * [`fn withPort(port)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgetwithport)
            * [`fn withScheme(scheme)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgetwithscheme)
            * [`obj spec.authProxyContainer.container.lifecycle.preStop.httpGet.httpHeaders`](#obj-specauthproxycontainercontainerlifecycleprestophttpgethttpheaders)
              * [`fn withName(name)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgethttpheaderswithname)
              * [`fn withValue(value)`](#fn-specauthproxycontainercontainerlifecycleprestophttpgethttpheaderswithvalue)
          * [`obj spec.authProxyContainer.container.lifecycle.preStop.tcpSocket`](#obj-specauthproxycontainercontainerlifecycleprestoptcpsocket)
            * [`fn withHost(host)`](#fn-specauthproxycontainercontainerlifecycleprestoptcpsocketwithhost)
            * [`fn withPort(port)`](#fn-specauthproxycontainercontainerlifecycleprestoptcpsocketwithport)
      * [`obj spec.authProxyContainer.container.livenessProbe`](#obj-specauthproxycontainercontainerlivenessprobe)
        * [`fn withFailureThreshold(failureThreshold)`](#fn-specauthproxycontainercontainerlivenessprobewithfailurethreshold)
        * [`fn withInitialDelaySeconds(initialDelaySeconds)`](#fn-specauthproxycontainercontainerlivenessprobewithinitialdelayseconds)
        * [`fn withPeriodSeconds(periodSeconds)`](#fn-specauthproxycontainercontainerlivenessprobewithperiodseconds)
        * [`fn withSuccessThreshold(successThreshold)`](#fn-specauthproxycontainercontainerlivenessprobewithsuccessthreshold)
        * [`fn withTerminationGracePeriodSeconds(terminationGracePeriodSeconds)`](#fn-specauthproxycontainercontainerlivenessprobewithterminationgraceperiodseconds)
        * [`fn withTimeoutSeconds(timeoutSeconds)`](#fn-specauthproxycontainercontainerlivenessprobewithtimeoutseconds)
        * [`obj spec.authProxyContainer.container.livenessProbe.exec`](#obj-specauthproxycontainercontainerlivenessprobeexec)
          * [`fn withCommand(command)`](#fn-specauthproxycontainercontainerlivenessprobeexecwithcommand)
          * [`fn withCommandMixin(command)`](#fn-specauthproxycontainercontainerlivenessprobeexecwithcommandmixin)
        * [`obj spec.authProxyContainer.container.livenessProbe.grpc`](#obj-specauthproxycontainercontainerlivenessprobegrpc)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerlivenessprobegrpcwithport)
          * [`fn withService(service)`](#fn-specauthproxycontainercontainerlivenessprobegrpcwithservice)
        * [`obj spec.authProxyContainer.container.livenessProbe.httpGet`](#obj-specauthproxycontainercontainerlivenessprobehttpget)
          * [`fn withHost(host)`](#fn-specauthproxycontainercontainerlivenessprobehttpgetwithhost)
          * [`fn withHttpHeaders(httpHeaders)`](#fn-specauthproxycontainercontainerlivenessprobehttpgetwithhttpheaders)
          * [`fn withHttpHeadersMixin(httpHeaders)`](#fn-specauthproxycontainercontainerlivenessprobehttpgetwithhttpheadersmixin)
          * [`fn withPath(path)`](#fn-specauthproxycontainercontainerlivenessprobehttpgetwithpath)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerlivenessprobehttpgetwithport)
          * [`fn withScheme(scheme)`](#fn-specauthproxycontainercontainerlivenessprobehttpgetwithscheme)
          * [`obj spec.authProxyContainer.container.livenessProbe.httpGet.httpHeaders`](#obj-specauthproxycontainercontainerlivenessprobehttpgethttpheaders)
            * [`fn withName(name)`](#fn-specauthproxycontainercontainerlivenessprobehttpgethttpheaderswithname)
            * [`fn withValue(value)`](#fn-specauthproxycontainercontainerlivenessprobehttpgethttpheaderswithvalue)
        * [`obj spec.authProxyContainer.container.livenessProbe.tcpSocket`](#obj-specauthproxycontainercontainerlivenessprobetcpsocket)
          * [`fn withHost(host)`](#fn-specauthproxycontainercontainerlivenessprobetcpsocketwithhost)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerlivenessprobetcpsocketwithport)
      * [`obj spec.authProxyContainer.container.ports`](#obj-specauthproxycontainercontainerports)
        * [`fn withContainerPort(containerPort)`](#fn-specauthproxycontainercontainerportswithcontainerport)
        * [`fn withHostIP(hostIP)`](#fn-specauthproxycontainercontainerportswithhostip)
        * [`fn withHostPort(hostPort)`](#fn-specauthproxycontainercontainerportswithhostport)
        * [`fn withName(name)`](#fn-specauthproxycontainercontainerportswithname)
        * [`fn withProtocol(protocol)`](#fn-specauthproxycontainercontainerportswithprotocol)
      * [`obj spec.authProxyContainer.container.readinessProbe`](#obj-specauthproxycontainercontainerreadinessprobe)
        * [`fn withFailureThreshold(failureThreshold)`](#fn-specauthproxycontainercontainerreadinessprobewithfailurethreshold)
        * [`fn withInitialDelaySeconds(initialDelaySeconds)`](#fn-specauthproxycontainercontainerreadinessprobewithinitialdelayseconds)
        * [`fn withPeriodSeconds(periodSeconds)`](#fn-specauthproxycontainercontainerreadinessprobewithperiodseconds)
        * [`fn withSuccessThreshold(successThreshold)`](#fn-specauthproxycontainercontainerreadinessprobewithsuccessthreshold)
        * [`fn withTerminationGracePeriodSeconds(terminationGracePeriodSeconds)`](#fn-specauthproxycontainercontainerreadinessprobewithterminationgraceperiodseconds)
        * [`fn withTimeoutSeconds(timeoutSeconds)`](#fn-specauthproxycontainercontainerreadinessprobewithtimeoutseconds)
        * [`obj spec.authProxyContainer.container.readinessProbe.exec`](#obj-specauthproxycontainercontainerreadinessprobeexec)
          * [`fn withCommand(command)`](#fn-specauthproxycontainercontainerreadinessprobeexecwithcommand)
          * [`fn withCommandMixin(command)`](#fn-specauthproxycontainercontainerreadinessprobeexecwithcommandmixin)
        * [`obj spec.authProxyContainer.container.readinessProbe.grpc`](#obj-specauthproxycontainercontainerreadinessprobegrpc)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerreadinessprobegrpcwithport)
          * [`fn withService(service)`](#fn-specauthproxycontainercontainerreadinessprobegrpcwithservice)
        * [`obj spec.authProxyContainer.container.readinessProbe.httpGet`](#obj-specauthproxycontainercontainerreadinessprobehttpget)
          * [`fn withHost(host)`](#fn-specauthproxycontainercontainerreadinessprobehttpgetwithhost)
          * [`fn withHttpHeaders(httpHeaders)`](#fn-specauthproxycontainercontainerreadinessprobehttpgetwithhttpheaders)
          * [`fn withHttpHeadersMixin(httpHeaders)`](#fn-specauthproxycontainercontainerreadinessprobehttpgetwithhttpheadersmixin)
          * [`fn withPath(path)`](#fn-specauthproxycontainercontainerreadinessprobehttpgetwithpath)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerreadinessprobehttpgetwithport)
          * [`fn withScheme(scheme)`](#fn-specauthproxycontainercontainerreadinessprobehttpgetwithscheme)
          * [`obj spec.authProxyContainer.container.readinessProbe.httpGet.httpHeaders`](#obj-specauthproxycontainercontainerreadinessprobehttpgethttpheaders)
            * [`fn withName(name)`](#fn-specauthproxycontainercontainerreadinessprobehttpgethttpheaderswithname)
            * [`fn withValue(value)`](#fn-specauthproxycontainercontainerreadinessprobehttpgethttpheaderswithvalue)
        * [`obj spec.authProxyContainer.container.readinessProbe.tcpSocket`](#obj-specauthproxycontainercontainerreadinessprobetcpsocket)
          * [`fn withHost(host)`](#fn-specauthproxycontainercontainerreadinessprobetcpsocketwithhost)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerreadinessprobetcpsocketwithport)
      * [`obj spec.authProxyContainer.container.resources`](#obj-specauthproxycontainercontainerresources)
        * [`fn withClaims(claims)`](#fn-specauthproxycontainercontainerresourceswithclaims)
        * [`fn withClaimsMixin(claims)`](#fn-specauthproxycontainercontainerresourceswithclaimsmixin)
        * [`fn withLimits(limits)`](#fn-specauthproxycontainercontainerresourceswithlimits)
        * [`fn withLimitsMixin(limits)`](#fn-specauthproxycontainercontainerresourceswithlimitsmixin)
        * [`fn withRequests(requests)`](#fn-specauthproxycontainercontainerresourceswithrequests)
        * [`fn withRequestsMixin(requests)`](#fn-specauthproxycontainercontainerresourceswithrequestsmixin)
        * [`obj spec.authProxyContainer.container.resources.claims`](#obj-specauthproxycontainercontainerresourcesclaims)
          * [`fn withName(name)`](#fn-specauthproxycontainercontainerresourcesclaimswithname)
      * [`obj spec.authProxyContainer.container.securityContext`](#obj-specauthproxycontainercontainersecuritycontext)
        * [`fn withAllowPrivilegeEscalation(allowPrivilegeEscalation)`](#fn-specauthproxycontainercontainersecuritycontextwithallowprivilegeescalation)
        * [`fn withPrivileged(privileged)`](#fn-specauthproxycontainercontainersecuritycontextwithprivileged)
        * [`fn withProcMount(procMount)`](#fn-specauthproxycontainercontainersecuritycontextwithprocmount)
        * [`fn withReadOnlyRootFilesystem(readOnlyRootFilesystem)`](#fn-specauthproxycontainercontainersecuritycontextwithreadonlyrootfilesystem)
        * [`fn withRunAsGroup(runAsGroup)`](#fn-specauthproxycontainercontainersecuritycontextwithrunasgroup)
        * [`fn withRunAsNonRoot(runAsNonRoot)`](#fn-specauthproxycontainercontainersecuritycontextwithrunasnonroot)
        * [`fn withRunAsUser(runAsUser)`](#fn-specauthproxycontainercontainersecuritycontextwithrunasuser)
        * [`obj spec.authProxyContainer.container.securityContext.capabilities`](#obj-specauthproxycontainercontainersecuritycontextcapabilities)
          * [`fn withAdd(add)`](#fn-specauthproxycontainercontainersecuritycontextcapabilitieswithadd)
          * [`fn withAddMixin(add)`](#fn-specauthproxycontainercontainersecuritycontextcapabilitieswithaddmixin)
          * [`fn withDrop(drop)`](#fn-specauthproxycontainercontainersecuritycontextcapabilitieswithdrop)
          * [`fn withDropMixin(drop)`](#fn-specauthproxycontainercontainersecuritycontextcapabilitieswithdropmixin)
        * [`obj spec.authProxyContainer.container.securityContext.seLinuxOptions`](#obj-specauthproxycontainercontainersecuritycontextselinuxoptions)
          * [`fn withLevel(level)`](#fn-specauthproxycontainercontainersecuritycontextselinuxoptionswithlevel)
          * [`fn withRole(role)`](#fn-specauthproxycontainercontainersecuritycontextselinuxoptionswithrole)
          * [`fn withType(type)`](#fn-specauthproxycontainercontainersecuritycontextselinuxoptionswithtype)
          * [`fn withUser(user)`](#fn-specauthproxycontainercontainersecuritycontextselinuxoptionswithuser)
        * [`obj spec.authProxyContainer.container.securityContext.seccompProfile`](#obj-specauthproxycontainercontainersecuritycontextseccompprofile)
          * [`fn withLocalhostProfile(localhostProfile)`](#fn-specauthproxycontainercontainersecuritycontextseccompprofilewithlocalhostprofile)
          * [`fn withType(type)`](#fn-specauthproxycontainercontainersecuritycontextseccompprofilewithtype)
        * [`obj spec.authProxyContainer.container.securityContext.windowsOptions`](#obj-specauthproxycontainercontainersecuritycontextwindowsoptions)
          * [`fn withGmsaCredentialSpec(gmsaCredentialSpec)`](#fn-specauthproxycontainercontainersecuritycontextwindowsoptionswithgmsacredentialspec)
          * [`fn withGmsaCredentialSpecName(gmsaCredentialSpecName)`](#fn-specauthproxycontainercontainersecuritycontextwindowsoptionswithgmsacredentialspecname)
          * [`fn withHostProcess(hostProcess)`](#fn-specauthproxycontainercontainersecuritycontextwindowsoptionswithhostprocess)
          * [`fn withRunAsUserName(runAsUserName)`](#fn-specauthproxycontainercontainersecuritycontextwindowsoptionswithrunasusername)
      * [`obj spec.authProxyContainer.container.startupProbe`](#obj-specauthproxycontainercontainerstartupprobe)
        * [`fn withFailureThreshold(failureThreshold)`](#fn-specauthproxycontainercontainerstartupprobewithfailurethreshold)
        * [`fn withInitialDelaySeconds(initialDelaySeconds)`](#fn-specauthproxycontainercontainerstartupprobewithinitialdelayseconds)
        * [`fn withPeriodSeconds(periodSeconds)`](#fn-specauthproxycontainercontainerstartupprobewithperiodseconds)
        * [`fn withSuccessThreshold(successThreshold)`](#fn-specauthproxycontainercontainerstartupprobewithsuccessthreshold)
        * [`fn withTerminationGracePeriodSeconds(terminationGracePeriodSeconds)`](#fn-specauthproxycontainercontainerstartupprobewithterminationgraceperiodseconds)
        * [`fn withTimeoutSeconds(timeoutSeconds)`](#fn-specauthproxycontainercontainerstartupprobewithtimeoutseconds)
        * [`obj spec.authProxyContainer.container.startupProbe.exec`](#obj-specauthproxycontainercontainerstartupprobeexec)
          * [`fn withCommand(command)`](#fn-specauthproxycontainercontainerstartupprobeexecwithcommand)
          * [`fn withCommandMixin(command)`](#fn-specauthproxycontainercontainerstartupprobeexecwithcommandmixin)
        * [`obj spec.authProxyContainer.container.startupProbe.grpc`](#obj-specauthproxycontainercontainerstartupprobegrpc)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerstartupprobegrpcwithport)
          * [`fn withService(service)`](#fn-specauthproxycontainercontainerstartupprobegrpcwithservice)
        * [`obj spec.authProxyContainer.container.startupProbe.httpGet`](#obj-specauthproxycontainercontainerstartupprobehttpget)
          * [`fn withHost(host)`](#fn-specauthproxycontainercontainerstartupprobehttpgetwithhost)
          * [`fn withHttpHeaders(httpHeaders)`](#fn-specauthproxycontainercontainerstartupprobehttpgetwithhttpheaders)
          * [`fn withHttpHeadersMixin(httpHeaders)`](#fn-specauthproxycontainercontainerstartupprobehttpgetwithhttpheadersmixin)
          * [`fn withPath(path)`](#fn-specauthproxycontainercontainerstartupprobehttpgetwithpath)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerstartupprobehttpgetwithport)
          * [`fn withScheme(scheme)`](#fn-specauthproxycontainercontainerstartupprobehttpgetwithscheme)
          * [`obj spec.authProxyContainer.container.startupProbe.httpGet.httpHeaders`](#obj-specauthproxycontainercontainerstartupprobehttpgethttpheaders)
            * [`fn withName(name)`](#fn-specauthproxycontainercontainerstartupprobehttpgethttpheaderswithname)
            * [`fn withValue(value)`](#fn-specauthproxycontainercontainerstartupprobehttpgethttpheaderswithvalue)
        * [`obj spec.authProxyContainer.container.startupProbe.tcpSocket`](#obj-specauthproxycontainercontainerstartupprobetcpsocket)
          * [`fn withHost(host)`](#fn-specauthproxycontainercontainerstartupprobetcpsocketwithhost)
          * [`fn withPort(port)`](#fn-specauthproxycontainercontainerstartupprobetcpsocketwithport)
      * [`obj spec.authProxyContainer.container.volumeDevices`](#obj-specauthproxycontainercontainervolumedevices)
        * [`fn withDevicePath(devicePath)`](#fn-specauthproxycontainercontainervolumedeviceswithdevicepath)
        * [`fn withName(name)`](#fn-specauthproxycontainercontainervolumedeviceswithname)
      * [`obj spec.authProxyContainer.container.volumeMounts`](#obj-specauthproxycontainercontainervolumemounts)
        * [`fn withMountPath(mountPath)`](#fn-specauthproxycontainercontainervolumemountswithmountpath)
        * [`fn withMountPropagation(mountPropagation)`](#fn-specauthproxycontainercontainervolumemountswithmountpropagation)
        * [`fn withName(name)`](#fn-specauthproxycontainercontainervolumemountswithname)
        * [`fn withReadOnly(readOnly)`](#fn-specauthproxycontainercontainervolumemountswithreadonly)
        * [`fn withSubPath(subPath)`](#fn-specauthproxycontainercontainervolumemountswithsubpath)
        * [`fn withSubPathExpr(subPathExpr)`](#fn-specauthproxycontainercontainervolumemountswithsubpathexpr)
    * [`obj spec.authProxyContainer.resources`](#obj-specauthproxycontainerresources)
      * [`fn withClaims(claims)`](#fn-specauthproxycontainerresourceswithclaims)
      * [`fn withClaimsMixin(claims)`](#fn-specauthproxycontainerresourceswithclaimsmixin)
      * [`fn withLimits(limits)`](#fn-specauthproxycontainerresourceswithlimits)
      * [`fn withLimitsMixin(limits)`](#fn-specauthproxycontainerresourceswithlimitsmixin)
      * [`fn withRequests(requests)`](#fn-specauthproxycontainerresourceswithrequests)
      * [`fn withRequestsMixin(requests)`](#fn-specauthproxycontainerresourceswithrequestsmixin)
      * [`obj spec.authProxyContainer.resources.claims`](#obj-specauthproxycontainerresourcesclaims)
        * [`fn withName(name)`](#fn-specauthproxycontainerresourcesclaimswithname)
    * [`obj spec.authProxyContainer.telemetry`](#obj-specauthproxycontainertelemetry)
      * [`fn withDisableMetrics(disableMetrics)`](#fn-specauthproxycontainertelemetrywithdisablemetrics)
      * [`fn withDisableTraces(disableTraces)`](#fn-specauthproxycontainertelemetrywithdisabletraces)
      * [`fn withHttpPort(httpPort)`](#fn-specauthproxycontainertelemetrywithhttpport)
      * [`fn withPrometheus(prometheus)`](#fn-specauthproxycontainertelemetrywithprometheus)
      * [`fn withPrometheusNamespace(prometheusNamespace)`](#fn-specauthproxycontainertelemetrywithprometheusnamespace)
      * [`fn withQuotaProject(quotaProject)`](#fn-specauthproxycontainertelemetrywithquotaproject)
      * [`fn withTelemetryPrefix(telemetryPrefix)`](#fn-specauthproxycontainertelemetrywithtelemetryprefix)
      * [`fn withTelemetryProject(telemetryProject)`](#fn-specauthproxycontainertelemetrywithtelemetryproject)
      * [`fn withTelemetrySampleRate(telemetrySampleRate)`](#fn-specauthproxycontainertelemetrywithtelemetrysamplerate)
  * [`obj spec.instances`](#obj-specinstances)
    * [`fn withAutoIAMAuthN(autoIAMAuthN)`](#fn-specinstanceswithautoiamauthn)
    * [`fn withConnectionString(connectionString)`](#fn-specinstanceswithconnectionstring)
    * [`fn withHostEnvName(hostEnvName)`](#fn-specinstanceswithhostenvname)
    * [`fn withPort(port)`](#fn-specinstanceswithport)
    * [`fn withPortEnvName(portEnvName)`](#fn-specinstanceswithportenvname)
    * [`fn withPrivateIP(privateIP)`](#fn-specinstanceswithprivateip)
    * [`fn withUnixSocketPath(unixSocketPath)`](#fn-specinstanceswithunixsocketpath)
    * [`fn withUnixSocketPathEnvName(unixSocketPathEnvName)`](#fn-specinstanceswithunixsocketpathenvname)
  * [`obj spec.workloadSelector`](#obj-specworkloadselector)
    * [`fn withKind(kind)`](#fn-specworkloadselectorwithkind)
    * [`fn withName(name)`](#fn-specworkloadselectorwithname)
    * [`obj spec.workloadSelector.selector`](#obj-specworkloadselectorselector)
      * [`fn withMatchExpressions(matchExpressions)`](#fn-specworkloadselectorselectorwithmatchexpressions)
      * [`fn withMatchExpressionsMixin(matchExpressions)`](#fn-specworkloadselectorselectorwithmatchexpressionsmixin)
      * [`fn withMatchLabels(matchLabels)`](#fn-specworkloadselectorselectorwithmatchlabels)
      * [`fn withMatchLabelsMixin(matchLabels)`](#fn-specworkloadselectorselectorwithmatchlabelsmixin)
      * [`obj spec.workloadSelector.selector.matchExpressions`](#obj-specworkloadselectorselectormatchexpressions)
        * [`fn withKey(key)`](#fn-specworkloadselectorselectormatchexpressionswithkey)
        * [`fn withOperator(operator)`](#fn-specworkloadselectorselectormatchexpressionswithoperator)
        * [`fn withValues(values)`](#fn-specworkloadselectorselectormatchexpressionswithvalues)
        * [`fn withValuesMixin(values)`](#fn-specworkloadselectorselectormatchexpressionswithvaluesmixin)

## Fields

### fn new

```ts
new(name)
```

new returns an instance of AuthProxyWorkload

## obj metadata

"ObjectMeta is metadata that all persisted resources must have, which includes all objects users must create."

### fn metadata.withAnnotations

```ts
withAnnotations(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

### fn metadata.withAnnotationsMixin

```ts
withAnnotationsMixin(annotations)
```

"Annotations is an unstructured key value map stored with a resource that may be set by external tools to store and retrieve arbitrary metadata. They are not queryable and should be preserved when modifying objects. More info: http://kubernetes.io/docs/user-guide/annotations"

**Note:** This function appends passed data to existing values

### fn metadata.withClusterName

```ts
withClusterName(clusterName)
```

"The name of the cluster which the object belongs to. This is used to distinguish resources with same name and namespace in different clusters. This field is not set anywhere right now and apiserver is going to ignore it if set in create or update request."

### fn metadata.withCreationTimestamp

```ts
withCreationTimestamp(creationTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withDeletionGracePeriodSeconds

```ts
withDeletionGracePeriodSeconds(deletionGracePeriodSeconds)
```

"Number of seconds allowed for this object to gracefully terminate before it will be removed from the system. Only set when deletionTimestamp is also set. May only be shortened. Read-only."

### fn metadata.withDeletionTimestamp

```ts
withDeletionTimestamp(deletionTimestamp)
```

"Time is a wrapper around time.Time which supports correct marshaling to YAML and JSON.  Wrappers are provided for many of the factory methods that the time package offers."

### fn metadata.withFinalizers

```ts
withFinalizers(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

### fn metadata.withFinalizersMixin

```ts
withFinalizersMixin(finalizers)
```

"Must be empty before the object is deleted from the registry. Each entry is an identifier for the responsible component that will remove the entry from the list. If the deletionTimestamp of the object is non-nil, entries in this list can only be removed. Finalizers may be processed and removed in any order.  Order is NOT enforced because it introduces significant risk of stuck finalizers. finalizers is a shared field, any actor with permission can reorder it. If the finalizer list is processed in order, then this can lead to a situation in which the component responsible for the first finalizer in the list is waiting for a signal (field value, external system, or other) produced by a component responsible for a finalizer later in the list, resulting in a deadlock. Without enforced ordering finalizers are free to order amongst themselves and are not vulnerable to ordering changes in the list."

**Note:** This function appends passed data to existing values

### fn metadata.withGenerateName

```ts
withGenerateName(generateName)
```

"GenerateName is an optional prefix, used by the server, to generate a unique name ONLY IF the Name field has not been provided. If this field is used, the name returned to the client will be different than the name passed. This value will also be combined with a unique suffix. The provided value has the same validation rules as the Name field, and may be truncated by the length of the suffix required to make the value unique on the server.\n\nIf this field is specified and the generated name exists, the server will NOT return a 409 - instead, it will either return 201 Created or 500 with Reason ServerTimeout indicating a unique name could not be found in the time allotted, and the client should retry (optionally after the time indicated in the Retry-After header).\n\nApplied only if Name is not specified. More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#idempotency"

### fn metadata.withGeneration

```ts
withGeneration(generation)
```

"A sequence number representing a specific generation of the desired state. Populated by the system. Read-only."

### fn metadata.withLabels

```ts
withLabels(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

### fn metadata.withLabelsMixin

```ts
withLabelsMixin(labels)
```

"Map of string keys and values that can be used to organize and categorize (scope and select) objects. May match selectors of replication controllers and services. More info: http://kubernetes.io/docs/user-guide/labels"

**Note:** This function appends passed data to existing values

### fn metadata.withName

```ts
withName(name)
```

"Name must be unique within a namespace. Is required when creating resources, although some resources may allow a client to request the generation of an appropriate name automatically. Name is primarily intended for creation idempotence and configuration definition. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/identifiers#names"

### fn metadata.withNamespace

```ts
withNamespace(namespace)
```

"Namespace defines the space within which each name must be unique. An empty namespace is equivalent to the \"default\" namespace, but \"default\" is the canonical representation. Not all objects are required to be scoped to a namespace - the value of this field for those objects will be empty.\n\nMust be a DNS_LABEL. Cannot be updated. More info: http://kubernetes.io/docs/user-guide/namespaces"

### fn metadata.withOwnerReferences

```ts
withOwnerReferences(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

### fn metadata.withOwnerReferencesMixin

```ts
withOwnerReferencesMixin(ownerReferences)
```

"List of objects depended by this object. If ALL objects in the list have been deleted, this object will be garbage collected. If this object is managed by a controller, then an entry in this list will point to this controller, with the controller field set to true. There cannot be more than one managing controller."

**Note:** This function appends passed data to existing values

### fn metadata.withResourceVersion

```ts
withResourceVersion(resourceVersion)
```

"An opaque value that represents the internal version of this object that can be used by clients to determine when objects have changed. May be used for optimistic concurrency, change detection, and the watch operation on a resource or set of resources. Clients must treat these values as opaque and passed unmodified back to the server. They may only be valid for a particular resource or set of resources.\n\nPopulated by the system. Read-only. Value must be treated as opaque by clients and . More info: https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#concurrency-control-and-consistency"

### fn metadata.withSelfLink

```ts
withSelfLink(selfLink)
```

"SelfLink is a URL representing this object. Populated by the system. Read-only.\n\nDEPRECATED Kubernetes will stop propagating this field in 1.20 release and the field is planned to be removed in 1.21 release."

### fn metadata.withUid

```ts
withUid(uid)
```

"UID is the unique in time and space value for this object. It is typically generated by the server on successful creation of a resource and is not allowed to change on PUT operations.\n\nPopulated by the system. Read-only. More info: http://kubernetes.io/docs/user-guide/identifiers#uids"

## obj spec

"AuthProxyWorkloadSpec describes where and how to configure the proxy."

### fn spec.withInstances

```ts
withInstances(instances)
```

"Instances describes the Cloud SQL instances to configure on the proxy container."

### fn spec.withInstancesMixin

```ts
withInstancesMixin(instances)
```

"Instances describes the Cloud SQL instances to configure on the proxy container."

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer

"AuthProxyContainer describes the resources and config for the Auth Proxy container."

### fn spec.authProxyContainer.withImage

```ts
withImage(image)
```

"Image is the URL to the proxy image. Optional, by default the operator will use the latest Cloud SQL Auth Proxy version as of the release of the operator. \n The operator ensures that all workloads configured with the default proxy image are upgraded automatically to use to the latest released proxy image. \n When the customer upgrades the operator, the operator upgrades all workloads using the default proxy image to the latest proxy image. The change to the proxy container image is applied in accordance with the RolloutStrategy."

### fn spec.authProxyContainer.withMaxConnections

```ts
withMaxConnections(maxConnections)
```

"MaxConnections limits the number of connections. Default value is no limit. This sets the proxy container's CLI argument `--max-connections`"

### fn spec.authProxyContainer.withMaxSigtermDelay

```ts
withMaxSigtermDelay(maxSigtermDelay)
```

"MaxSigtermDelay is the maximum number of seconds to wait for connections to close after receiving a TERM signal. This sets the proxy container's CLI argument `--max-sigterm-delay` and configures `terminationGracePeriodSeconds` on the workload's PodSpec."

### fn spec.authProxyContainer.withRolloutStrategy

```ts
withRolloutStrategy(rolloutStrategy)
```

"RolloutStrategy indicates the strategy to use when rolling out changes to the workloads affected by the results. When this is set to `Workload`, changes to this resource will be automatically applied to a running Deployment, StatefulSet, DaemonSet, or ReplicaSet in accordance with the Strategy set on that workload. When this is set to `None`, the operator will take no action to roll out changes to affected workloads. `Workload` will be used by default if no value is set. See: https://kubernetes.io/docs/concepts/workloads/controllers/deployment/#strategy"

### fn spec.authProxyContainer.withSqlAdminAPIEndpoint

```ts
withSqlAdminAPIEndpoint(sqlAdminAPIEndpoint)
```

"SQLAdminAPIEndpoint is a debugging parameter that when specified will change the Google Cloud api endpoint used by the proxy."

## obj spec.authProxyContainer.adminServer

"AdminServer specifies the config for the proxy's admin service which is available to other containers in the same pod."

### fn spec.authProxyContainer.adminServer.withEnableAPIs

```ts
withEnableAPIs(enableAPIs)
```

"EnableAPIs specifies the list of admin APIs to enable. At least one API must be enabled. Possible values: - \"Debug\" will enable pprof debugging by setting the `--debug` cli flag. - \"QuitQuitQuit\" will enable pprof debugging by setting the `--quitquitquit` cli flag."

### fn spec.authProxyContainer.adminServer.withEnableAPIsMixin

```ts
withEnableAPIsMixin(enableAPIs)
```

"EnableAPIs specifies the list of admin APIs to enable. At least one API must be enabled. Possible values: - \"Debug\" will enable pprof debugging by setting the `--debug` cli flag. - \"QuitQuitQuit\" will enable pprof debugging by setting the `--quitquitquit` cli flag."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.adminServer.withPort

```ts
withPort(port)
```

"Port the port for the proxy's localhost-only admin server. This sets the proxy container's CLI argument `--admin-port`"

## obj spec.authProxyContainer.container

"Container is debugging parameter that when specified will override the proxy container with a completely custom Container spec."

### fn spec.authProxyContainer.container.withArgs

```ts
withArgs(args)
```

"Arguments to the entrypoint. The container image's CMD is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \"$$(VAR_NAME)\" will produce the string literal \"$(VAR_NAME)\". Escaped references will never be expanded, regardless of whether the variable exists or not. Cannot be updated. More info: https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell"

### fn spec.authProxyContainer.container.withArgsMixin

```ts
withArgsMixin(args)
```

"Arguments to the entrypoint. The container image's CMD is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \"$$(VAR_NAME)\" will produce the string literal \"$(VAR_NAME)\". Escaped references will never be expanded, regardless of whether the variable exists or not. Cannot be updated. More info: https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell"

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.withCommand

```ts
withCommand(command)
```

"Entrypoint array. Not executed within a shell. The container image's ENTRYPOINT is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \"$$(VAR_NAME)\" will produce the string literal \"$(VAR_NAME)\". Escaped references will never be expanded, regardless of whether the variable exists or not. Cannot be updated. More info: https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell"

### fn spec.authProxyContainer.container.withCommandMixin

```ts
withCommandMixin(command)
```

"Entrypoint array. Not executed within a shell. The container image's ENTRYPOINT is used if this is not provided. Variable references $(VAR_NAME) are expanded using the container's environment. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \"$$(VAR_NAME)\" will produce the string literal \"$(VAR_NAME)\". Escaped references will never be expanded, regardless of whether the variable exists or not. Cannot be updated. More info: https://kubernetes.io/docs/tasks/inject-data-application/define-command-argument-container/#running-a-command-in-a-shell"

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.withEnv

```ts
withEnv(env)
```

"List of environment variables to set in the container. Cannot be updated."

### fn spec.authProxyContainer.container.withEnvFrom

```ts
withEnvFrom(envFrom)
```

"List of sources to populate environment variables in the container. The keys defined within a source must be a C_IDENTIFIER. All invalid keys will be reported as an event when the container is starting. When a key exists in multiple sources, the value associated with the last source will take precedence. Values defined by an Env with a duplicate key will take precedence. Cannot be updated."

### fn spec.authProxyContainer.container.withEnvFromMixin

```ts
withEnvFromMixin(envFrom)
```

"List of sources to populate environment variables in the container. The keys defined within a source must be a C_IDENTIFIER. All invalid keys will be reported as an event when the container is starting. When a key exists in multiple sources, the value associated with the last source will take precedence. Values defined by an Env with a duplicate key will take precedence. Cannot be updated."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.withEnvMixin

```ts
withEnvMixin(env)
```

"List of environment variables to set in the container. Cannot be updated."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.withImage

```ts
withImage(image)
```

"Container image name. More info: https://kubernetes.io/docs/concepts/containers/images This field is optional to allow higher level config management to default or override container images in workload controllers like Deployments and StatefulSets."

### fn spec.authProxyContainer.container.withImagePullPolicy

```ts
withImagePullPolicy(imagePullPolicy)
```

"Image pull policy. One of Always, Never, IfNotPresent. Defaults to Always if :latest tag is specified, or IfNotPresent otherwise. Cannot be updated. More info: https://kubernetes.io/docs/concepts/containers/images#updating-images"

### fn spec.authProxyContainer.container.withName

```ts
withName(name)
```

"Name of the container specified as a DNS_LABEL. Each container in a pod must have a unique name (DNS_LABEL). Cannot be updated."

### fn spec.authProxyContainer.container.withPorts

```ts
withPorts(ports)
```

"List of ports to expose from the container. Not specifying a port here DOES NOT prevent that port from being exposed. Any port which is listening on the default \"0.0.0.0\" address inside a container will be accessible from the network. Modifying this array with strategic merge patch may corrupt the data. For more information See https://github.com/kubernetes/kubernetes/issues/108255. Cannot be updated."

### fn spec.authProxyContainer.container.withPortsMixin

```ts
withPortsMixin(ports)
```

"List of ports to expose from the container. Not specifying a port here DOES NOT prevent that port from being exposed. Any port which is listening on the default \"0.0.0.0\" address inside a container will be accessible from the network. Modifying this array with strategic merge patch may corrupt the data. For more information See https://github.com/kubernetes/kubernetes/issues/108255. Cannot be updated."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.withStdin

```ts
withStdin(stdin)
```

"Whether this container should allocate a buffer for stdin in the container runtime. If this is not set, reads from stdin in the container will always result in EOF. Default is false."

### fn spec.authProxyContainer.container.withStdinOnce

```ts
withStdinOnce(stdinOnce)
```

"Whether the container runtime should close the stdin channel after it has been opened by a single attach. When stdin is true the stdin stream will remain open across multiple attach sessions. If stdinOnce is set to true, stdin is opened on container start, is empty until the first client attaches to stdin, and then remains open and accepts data until the client disconnects, at which time stdin is closed and remains closed until the container is restarted. If this flag is false, a container processes that reads from stdin will never receive an EOF. Default is false"

### fn spec.authProxyContainer.container.withTerminationMessagePath

```ts
withTerminationMessagePath(terminationMessagePath)
```

"Optional: Path at which the file to which the container's termination message will be written is mounted into the container's filesystem. Message written is intended to be brief final status, such as an assertion failure message. Will be truncated by the node if greater than 4096 bytes. The total message length across all containers will be limited to 12kb. Defaults to /dev/termination-log. Cannot be updated."

### fn spec.authProxyContainer.container.withTerminationMessagePolicy

```ts
withTerminationMessagePolicy(terminationMessagePolicy)
```

"Indicate how the termination message should be populated. File will use the contents of terminationMessagePath to populate the container status message on both success and failure. FallbackToLogsOnError will use the last chunk of container log output if the termination message file is empty and the container exited with an error. The log output is limited to 2048 bytes or 80 lines, whichever is smaller. Defaults to File. Cannot be updated."

### fn spec.authProxyContainer.container.withTty

```ts
withTty(tty)
```

"Whether this container should allocate a TTY for itself, also requires 'stdin' to be true. Default is false."

### fn spec.authProxyContainer.container.withVolumeDevices

```ts
withVolumeDevices(volumeDevices)
```

"volumeDevices is the list of block devices to be used by the container."

### fn spec.authProxyContainer.container.withVolumeDevicesMixin

```ts
withVolumeDevicesMixin(volumeDevices)
```

"volumeDevices is the list of block devices to be used by the container."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.withVolumeMounts

```ts
withVolumeMounts(volumeMounts)
```

"Pod volumes to mount into the container's filesystem. Cannot be updated."

### fn spec.authProxyContainer.container.withVolumeMountsMixin

```ts
withVolumeMountsMixin(volumeMounts)
```

"Pod volumes to mount into the container's filesystem. Cannot be updated."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.withWorkingDir

```ts
withWorkingDir(workingDir)
```

"Container's working directory. If not specified, the container runtime's default will be used, which might be configured in the container image. Cannot be updated."

## obj spec.authProxyContainer.container.env

"List of environment variables to set in the container. Cannot be updated."

### fn spec.authProxyContainer.container.env.withName

```ts
withName(name)
```

"Name of the environment variable. Must be a C_IDENTIFIER."

### fn spec.authProxyContainer.container.env.withValue

```ts
withValue(value)
```

"Variable references $(VAR_NAME) are expanded using the previously defined environment variables in the container and any service environment variables. If a variable cannot be resolved, the reference in the input string will be unchanged. Double $$ are reduced to a single $, which allows for escaping the $(VAR_NAME) syntax: i.e. \"$$(VAR_NAME)\" will produce the string literal \"$(VAR_NAME)\". Escaped references will never be expanded, regardless of whether the variable exists or not. Defaults to \"\"."

## obj spec.authProxyContainer.container.env.valueFrom

"Source for the environment variable's value. Cannot be used if value is not empty."

## obj spec.authProxyContainer.container.env.valueFrom.configMapKeyRef

"Selects a key of a ConfigMap."

### fn spec.authProxyContainer.container.env.valueFrom.configMapKeyRef.withKey

```ts
withKey(key)
```

"The key to select."

### fn spec.authProxyContainer.container.env.valueFrom.configMapKeyRef.withName

```ts
withName(name)
```

"Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names TODO: Add other useful fields. apiVersion, kind, uid?"

### fn spec.authProxyContainer.container.env.valueFrom.configMapKeyRef.withOptional

```ts
withOptional(optional)
```

"Specify whether the ConfigMap or its key must be defined"

## obj spec.authProxyContainer.container.env.valueFrom.fieldRef

"Selects a field of the pod: supports metadata.name, metadata.namespace, `metadata.labels['<KEY>']`, `metadata.annotations['<KEY>']`, spec.nodeName, spec.serviceAccountName, status.hostIP, status.podIP, status.podIPs."

### fn spec.authProxyContainer.container.env.valueFrom.fieldRef.withApiVersion

```ts
withApiVersion(apiVersion)
```

"Version of the schema the FieldPath is written in terms of, defaults to \"v1\"."

### fn spec.authProxyContainer.container.env.valueFrom.fieldRef.withFieldPath

```ts
withFieldPath(fieldPath)
```

"Path of the field to select in the specified API version."

## obj spec.authProxyContainer.container.env.valueFrom.resourceFieldRef

"Selects a resource of the container: only resources limits and requests (limits.cpu, limits.memory, limits.ephemeral-storage, requests.cpu, requests.memory and requests.ephemeral-storage) are currently supported."

### fn spec.authProxyContainer.container.env.valueFrom.resourceFieldRef.withContainerName

```ts
withContainerName(containerName)
```

"Container name: required for volumes, optional for env vars"

### fn spec.authProxyContainer.container.env.valueFrom.resourceFieldRef.withDivisor

```ts
withDivisor(divisor)
```

"Specifies the output format of the exposed resources, defaults to \"1\

### fn spec.authProxyContainer.container.env.valueFrom.resourceFieldRef.withResource

```ts
withResource(resource)
```

"Required: resource to select"

## obj spec.authProxyContainer.container.env.valueFrom.secretKeyRef

"Selects a key of a secret in the pod's namespace"

### fn spec.authProxyContainer.container.env.valueFrom.secretKeyRef.withKey

```ts
withKey(key)
```

"The key of the secret to select from.  Must be a valid secret key."

### fn spec.authProxyContainer.container.env.valueFrom.secretKeyRef.withName

```ts
withName(name)
```

"Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names TODO: Add other useful fields. apiVersion, kind, uid?"

### fn spec.authProxyContainer.container.env.valueFrom.secretKeyRef.withOptional

```ts
withOptional(optional)
```

"Specify whether the Secret or its key must be defined"

## obj spec.authProxyContainer.container.envFrom

"List of sources to populate environment variables in the container. The keys defined within a source must be a C_IDENTIFIER. All invalid keys will be reported as an event when the container is starting. When a key exists in multiple sources, the value associated with the last source will take precedence. Values defined by an Env with a duplicate key will take precedence. Cannot be updated."

### fn spec.authProxyContainer.container.envFrom.withPrefix

```ts
withPrefix(prefix)
```

"An optional identifier to prepend to each key in the ConfigMap. Must be a C_IDENTIFIER."

## obj spec.authProxyContainer.container.envFrom.configMapRef

"The ConfigMap to select from"

### fn spec.authProxyContainer.container.envFrom.configMapRef.withName

```ts
withName(name)
```

"Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names TODO: Add other useful fields. apiVersion, kind, uid?"

### fn spec.authProxyContainer.container.envFrom.configMapRef.withOptional

```ts
withOptional(optional)
```

"Specify whether the ConfigMap must be defined"

## obj spec.authProxyContainer.container.envFrom.secretRef

"The Secret to select from"

### fn spec.authProxyContainer.container.envFrom.secretRef.withName

```ts
withName(name)
```

"Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names TODO: Add other useful fields. apiVersion, kind, uid?"

### fn spec.authProxyContainer.container.envFrom.secretRef.withOptional

```ts
withOptional(optional)
```

"Specify whether the Secret must be defined"

## obj spec.authProxyContainer.container.lifecycle

"Actions that the management system should take in response to container lifecycle events. Cannot be updated."

## obj spec.authProxyContainer.container.lifecycle.postStart

"PostStart is called immediately after a container is created. If the handler fails, the container is terminated and restarted according to its restart policy. Other management of the container blocks until the hook completes. More info: https://kubernetes.io/docs/concepts/containers/container-lifecycle-hooks/#container-hooks"

## obj spec.authProxyContainer.container.lifecycle.postStart.exec

"Exec specifies the action to take."

### fn spec.authProxyContainer.container.lifecycle.postStart.exec.withCommand

```ts
withCommand(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

### fn spec.authProxyContainer.container.lifecycle.postStart.exec.withCommandMixin

```ts
withCommandMixin(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.container.lifecycle.postStart.httpGet

"HTTPGet specifies the http request to perform."

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.withHost

```ts
withHost(host)
```

"Host name to connect to, defaults to the pod IP. You probably want to set \"Host\" in httpHeaders instead."

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.withHttpHeaders

```ts
withHttpHeaders(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.withHttpHeadersMixin

```ts
withHttpHeadersMixin(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.withPath

```ts
withPath(path)
```

"Path to access on the HTTP server."

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.withPort

```ts
withPort(port)
```

"Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.withScheme

```ts
withScheme(scheme)
```

"Scheme to use for connecting to the host. Defaults to HTTP."

## obj spec.authProxyContainer.container.lifecycle.postStart.httpGet.httpHeaders

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.httpHeaders.withName

```ts
withName(name)
```

"The header field name"

### fn spec.authProxyContainer.container.lifecycle.postStart.httpGet.httpHeaders.withValue

```ts
withValue(value)
```

"The header field value"

## obj spec.authProxyContainer.container.lifecycle.postStart.tcpSocket

"Deprecated. TCPSocket is NOT supported as a LifecycleHandler and kept for the backward compatibility. There are no validation of this field and lifecycle hooks will fail in runtime when tcp handler is specified."

### fn spec.authProxyContainer.container.lifecycle.postStart.tcpSocket.withHost

```ts
withHost(host)
```

"Optional: Host name to connect to, defaults to the pod IP."

### fn spec.authProxyContainer.container.lifecycle.postStart.tcpSocket.withPort

```ts
withPort(port)
```

"Number or name of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

## obj spec.authProxyContainer.container.lifecycle.preStop

"PreStop is called immediately before a container is terminated due to an API request or management event such as liveness/startup probe failure, preemption, resource contention, etc. The handler is not called if the container crashes or exits. The Pod's termination grace period countdown begins before the PreStop hook is executed. Regardless of the outcome of the handler, the container will eventually terminate within the Pod's termination grace period (unless delayed by finalizers). Other management of the container blocks until the hook completes or until the termination grace period is reached. More info: https://kubernetes.io/docs/concepts/containers/container-lifecycle-hooks/#container-hooks"

## obj spec.authProxyContainer.container.lifecycle.preStop.exec

"Exec specifies the action to take."

### fn spec.authProxyContainer.container.lifecycle.preStop.exec.withCommand

```ts
withCommand(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

### fn spec.authProxyContainer.container.lifecycle.preStop.exec.withCommandMixin

```ts
withCommandMixin(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.container.lifecycle.preStop.httpGet

"HTTPGet specifies the http request to perform."

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.withHost

```ts
withHost(host)
```

"Host name to connect to, defaults to the pod IP. You probably want to set \"Host\" in httpHeaders instead."

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.withHttpHeaders

```ts
withHttpHeaders(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.withHttpHeadersMixin

```ts
withHttpHeadersMixin(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.withPath

```ts
withPath(path)
```

"Path to access on the HTTP server."

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.withPort

```ts
withPort(port)
```

"Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.withScheme

```ts
withScheme(scheme)
```

"Scheme to use for connecting to the host. Defaults to HTTP."

## obj spec.authProxyContainer.container.lifecycle.preStop.httpGet.httpHeaders

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.httpHeaders.withName

```ts
withName(name)
```

"The header field name"

### fn spec.authProxyContainer.container.lifecycle.preStop.httpGet.httpHeaders.withValue

```ts
withValue(value)
```

"The header field value"

## obj spec.authProxyContainer.container.lifecycle.preStop.tcpSocket

"Deprecated. TCPSocket is NOT supported as a LifecycleHandler and kept for the backward compatibility. There are no validation of this field and lifecycle hooks will fail in runtime when tcp handler is specified."

### fn spec.authProxyContainer.container.lifecycle.preStop.tcpSocket.withHost

```ts
withHost(host)
```

"Optional: Host name to connect to, defaults to the pod IP."

### fn spec.authProxyContainer.container.lifecycle.preStop.tcpSocket.withPort

```ts
withPort(port)
```

"Number or name of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

## obj spec.authProxyContainer.container.livenessProbe

"Periodic probe of container liveness. Container will be restarted if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

### fn spec.authProxyContainer.container.livenessProbe.withFailureThreshold

```ts
withFailureThreshold(failureThreshold)
```

"Minimum consecutive failures for the probe to be considered failed after having succeeded. Defaults to 3. Minimum value is 1."

### fn spec.authProxyContainer.container.livenessProbe.withInitialDelaySeconds

```ts
withInitialDelaySeconds(initialDelaySeconds)
```

"Number of seconds after the container has started before liveness probes are initiated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

### fn spec.authProxyContainer.container.livenessProbe.withPeriodSeconds

```ts
withPeriodSeconds(periodSeconds)
```

"How often (in seconds) to perform the probe. Default to 10 seconds. Minimum value is 1."

### fn spec.authProxyContainer.container.livenessProbe.withSuccessThreshold

```ts
withSuccessThreshold(successThreshold)
```

"Minimum consecutive successes for the probe to be considered successful after having failed. Defaults to 1. Must be 1 for liveness and startup. Minimum value is 1."

### fn spec.authProxyContainer.container.livenessProbe.withTerminationGracePeriodSeconds

```ts
withTerminationGracePeriodSeconds(terminationGracePeriodSeconds)
```

"Optional duration in seconds the pod needs to terminate gracefully upon probe failure. The grace period is the duration in seconds after the processes running in the pod are sent a termination signal and the time when the processes are forcibly halted with a kill signal. Set this value longer than the expected cleanup time for your process. If this value is nil, the pod's terminationGracePeriodSeconds will be used. Otherwise, this value overrides the value provided by the pod spec. Value must be non-negative integer. The value zero indicates stop immediately via the kill signal (no opportunity to shut down). This is a beta field and requires enabling ProbeTerminationGracePeriod feature gate. Minimum value is 1. spec.terminationGracePeriodSeconds is used if unset."

### fn spec.authProxyContainer.container.livenessProbe.withTimeoutSeconds

```ts
withTimeoutSeconds(timeoutSeconds)
```

"Number of seconds after which the probe times out. Defaults to 1 second. Minimum value is 1. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

## obj spec.authProxyContainer.container.livenessProbe.exec

"Exec specifies the action to take."

### fn spec.authProxyContainer.container.livenessProbe.exec.withCommand

```ts
withCommand(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

### fn spec.authProxyContainer.container.livenessProbe.exec.withCommandMixin

```ts
withCommandMixin(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.container.livenessProbe.grpc

"GRPC specifies an action involving a GRPC port. This is a beta field and requires enabling GRPCContainerProbe feature gate."

### fn spec.authProxyContainer.container.livenessProbe.grpc.withPort

```ts
withPort(port)
```

"Port number of the gRPC service. Number must be in the range 1 to 65535."

### fn spec.authProxyContainer.container.livenessProbe.grpc.withService

```ts
withService(service)
```

"Service is the name of the service to place in the gRPC HealthCheckRequest (see https://github.com/grpc/grpc/blob/master/doc/health-checking.md). \n If this is not specified, the default behavior is defined by gRPC."

## obj spec.authProxyContainer.container.livenessProbe.httpGet

"HTTPGet specifies the http request to perform."

### fn spec.authProxyContainer.container.livenessProbe.httpGet.withHost

```ts
withHost(host)
```

"Host name to connect to, defaults to the pod IP. You probably want to set \"Host\" in httpHeaders instead."

### fn spec.authProxyContainer.container.livenessProbe.httpGet.withHttpHeaders

```ts
withHttpHeaders(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.livenessProbe.httpGet.withHttpHeadersMixin

```ts
withHttpHeadersMixin(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.livenessProbe.httpGet.withPath

```ts
withPath(path)
```

"Path to access on the HTTP server."

### fn spec.authProxyContainer.container.livenessProbe.httpGet.withPort

```ts
withPort(port)
```

"Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

### fn spec.authProxyContainer.container.livenessProbe.httpGet.withScheme

```ts
withScheme(scheme)
```

"Scheme to use for connecting to the host. Defaults to HTTP."

## obj spec.authProxyContainer.container.livenessProbe.httpGet.httpHeaders

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.livenessProbe.httpGet.httpHeaders.withName

```ts
withName(name)
```

"The header field name"

### fn spec.authProxyContainer.container.livenessProbe.httpGet.httpHeaders.withValue

```ts
withValue(value)
```

"The header field value"

## obj spec.authProxyContainer.container.livenessProbe.tcpSocket

"TCPSocket specifies an action involving a TCP port."

### fn spec.authProxyContainer.container.livenessProbe.tcpSocket.withHost

```ts
withHost(host)
```

"Optional: Host name to connect to, defaults to the pod IP."

### fn spec.authProxyContainer.container.livenessProbe.tcpSocket.withPort

```ts
withPort(port)
```

"Number or name of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

## obj spec.authProxyContainer.container.ports

"List of ports to expose from the container. Not specifying a port here DOES NOT prevent that port from being exposed. Any port which is listening on the default \"0.0.0.0\" address inside a container will be accessible from the network. Modifying this array with strategic merge patch may corrupt the data. For more information See https://github.com/kubernetes/kubernetes/issues/108255. Cannot be updated."

### fn spec.authProxyContainer.container.ports.withContainerPort

```ts
withContainerPort(containerPort)
```

"Number of port to expose on the pod's IP address. This must be a valid port number, 0 < x < 65536."

### fn spec.authProxyContainer.container.ports.withHostIP

```ts
withHostIP(hostIP)
```

"What host IP to bind the external port to."

### fn spec.authProxyContainer.container.ports.withHostPort

```ts
withHostPort(hostPort)
```

"Number of port to expose on the host. If specified, this must be a valid port number, 0 < x < 65536. If HostNetwork is specified, this must match ContainerPort. Most containers do not need this."

### fn spec.authProxyContainer.container.ports.withName

```ts
withName(name)
```

"If specified, this must be an IANA_SVC_NAME and unique within the pod. Each named port in a pod must have a unique name. Name for the port that can be referred to by services."

### fn spec.authProxyContainer.container.ports.withProtocol

```ts
withProtocol(protocol)
```

"Protocol for port. Must be UDP, TCP, or SCTP. Defaults to \"TCP\"."

## obj spec.authProxyContainer.container.readinessProbe

"Periodic probe of container service readiness. Container will be removed from service endpoints if the probe fails. Cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

### fn spec.authProxyContainer.container.readinessProbe.withFailureThreshold

```ts
withFailureThreshold(failureThreshold)
```

"Minimum consecutive failures for the probe to be considered failed after having succeeded. Defaults to 3. Minimum value is 1."

### fn spec.authProxyContainer.container.readinessProbe.withInitialDelaySeconds

```ts
withInitialDelaySeconds(initialDelaySeconds)
```

"Number of seconds after the container has started before liveness probes are initiated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

### fn spec.authProxyContainer.container.readinessProbe.withPeriodSeconds

```ts
withPeriodSeconds(periodSeconds)
```

"How often (in seconds) to perform the probe. Default to 10 seconds. Minimum value is 1."

### fn spec.authProxyContainer.container.readinessProbe.withSuccessThreshold

```ts
withSuccessThreshold(successThreshold)
```

"Minimum consecutive successes for the probe to be considered successful after having failed. Defaults to 1. Must be 1 for liveness and startup. Minimum value is 1."

### fn spec.authProxyContainer.container.readinessProbe.withTerminationGracePeriodSeconds

```ts
withTerminationGracePeriodSeconds(terminationGracePeriodSeconds)
```

"Optional duration in seconds the pod needs to terminate gracefully upon probe failure. The grace period is the duration in seconds after the processes running in the pod are sent a termination signal and the time when the processes are forcibly halted with a kill signal. Set this value longer than the expected cleanup time for your process. If this value is nil, the pod's terminationGracePeriodSeconds will be used. Otherwise, this value overrides the value provided by the pod spec. Value must be non-negative integer. The value zero indicates stop immediately via the kill signal (no opportunity to shut down). This is a beta field and requires enabling ProbeTerminationGracePeriod feature gate. Minimum value is 1. spec.terminationGracePeriodSeconds is used if unset."

### fn spec.authProxyContainer.container.readinessProbe.withTimeoutSeconds

```ts
withTimeoutSeconds(timeoutSeconds)
```

"Number of seconds after which the probe times out. Defaults to 1 second. Minimum value is 1. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

## obj spec.authProxyContainer.container.readinessProbe.exec

"Exec specifies the action to take."

### fn spec.authProxyContainer.container.readinessProbe.exec.withCommand

```ts
withCommand(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

### fn spec.authProxyContainer.container.readinessProbe.exec.withCommandMixin

```ts
withCommandMixin(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.container.readinessProbe.grpc

"GRPC specifies an action involving a GRPC port. This is a beta field and requires enabling GRPCContainerProbe feature gate."

### fn spec.authProxyContainer.container.readinessProbe.grpc.withPort

```ts
withPort(port)
```

"Port number of the gRPC service. Number must be in the range 1 to 65535."

### fn spec.authProxyContainer.container.readinessProbe.grpc.withService

```ts
withService(service)
```

"Service is the name of the service to place in the gRPC HealthCheckRequest (see https://github.com/grpc/grpc/blob/master/doc/health-checking.md). \n If this is not specified, the default behavior is defined by gRPC."

## obj spec.authProxyContainer.container.readinessProbe.httpGet

"HTTPGet specifies the http request to perform."

### fn spec.authProxyContainer.container.readinessProbe.httpGet.withHost

```ts
withHost(host)
```

"Host name to connect to, defaults to the pod IP. You probably want to set \"Host\" in httpHeaders instead."

### fn spec.authProxyContainer.container.readinessProbe.httpGet.withHttpHeaders

```ts
withHttpHeaders(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.readinessProbe.httpGet.withHttpHeadersMixin

```ts
withHttpHeadersMixin(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.readinessProbe.httpGet.withPath

```ts
withPath(path)
```

"Path to access on the HTTP server."

### fn spec.authProxyContainer.container.readinessProbe.httpGet.withPort

```ts
withPort(port)
```

"Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

### fn spec.authProxyContainer.container.readinessProbe.httpGet.withScheme

```ts
withScheme(scheme)
```

"Scheme to use for connecting to the host. Defaults to HTTP."

## obj spec.authProxyContainer.container.readinessProbe.httpGet.httpHeaders

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.readinessProbe.httpGet.httpHeaders.withName

```ts
withName(name)
```

"The header field name"

### fn spec.authProxyContainer.container.readinessProbe.httpGet.httpHeaders.withValue

```ts
withValue(value)
```

"The header field value"

## obj spec.authProxyContainer.container.readinessProbe.tcpSocket

"TCPSocket specifies an action involving a TCP port."

### fn spec.authProxyContainer.container.readinessProbe.tcpSocket.withHost

```ts
withHost(host)
```

"Optional: Host name to connect to, defaults to the pod IP."

### fn spec.authProxyContainer.container.readinessProbe.tcpSocket.withPort

```ts
withPort(port)
```

"Number or name of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

## obj spec.authProxyContainer.container.resources

"Compute Resources required by this container. Cannot be updated. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

### fn spec.authProxyContainer.container.resources.withClaims

```ts
withClaims(claims)
```

"Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. \n This is an alpha field and requires enabling the DynamicResourceAllocation feature gate. \n This field is immutable. It can only be set for containers."

### fn spec.authProxyContainer.container.resources.withClaimsMixin

```ts
withClaimsMixin(claims)
```

"Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. \n This is an alpha field and requires enabling the DynamicResourceAllocation feature gate. \n This field is immutable. It can only be set for containers."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.resources.withLimits

```ts
withLimits(limits)
```

"Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

### fn spec.authProxyContainer.container.resources.withLimitsMixin

```ts
withLimitsMixin(limits)
```

"Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.resources.withRequests

```ts
withRequests(requests)
```

"Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defined value. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

### fn spec.authProxyContainer.container.resources.withRequestsMixin

```ts
withRequestsMixin(requests)
```

"Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defined value. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.container.resources.claims

"Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. \n This is an alpha field and requires enabling the DynamicResourceAllocation feature gate. \n This field is immutable. It can only be set for containers."

### fn spec.authProxyContainer.container.resources.claims.withName

```ts
withName(name)
```

"Name must match the name of one entry in pod.spec.resourceClaims of the Pod where this field is used. It makes that resource available inside a container."

## obj spec.authProxyContainer.container.securityContext

"SecurityContext defines the security options the container should be run with. If set, the fields of SecurityContext override the equivalent fields of PodSecurityContext. More info: https://kubernetes.io/docs/tasks/configure-pod-container/security-context/"

### fn spec.authProxyContainer.container.securityContext.withAllowPrivilegeEscalation

```ts
withAllowPrivilegeEscalation(allowPrivilegeEscalation)
```

"AllowPrivilegeEscalation controls whether a process can gain more privileges than its parent process. This bool directly controls if the no_new_privs flag will be set on the container process. AllowPrivilegeEscalation is true always when the container is: 1) run as Privileged 2) has CAP_SYS_ADMIN Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.withPrivileged

```ts
withPrivileged(privileged)
```

"Run container in privileged mode. Processes in privileged containers are essentially equivalent to root on the host. Defaults to false. Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.withProcMount

```ts
withProcMount(procMount)
```

"procMount denotes the type of proc mount to use for the containers. The default is DefaultProcMount which uses the container runtime defaults for readonly paths and masked paths. This requires the ProcMountType feature flag to be enabled. Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.withReadOnlyRootFilesystem

```ts
withReadOnlyRootFilesystem(readOnlyRootFilesystem)
```

"Whether this container has a read-only root filesystem. Default is false. Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.withRunAsGroup

```ts
withRunAsGroup(runAsGroup)
```

"The GID to run the entrypoint of the container process. Uses runtime default if unset. May also be set in PodSecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence. Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.withRunAsNonRoot

```ts
withRunAsNonRoot(runAsNonRoot)
```

"Indicates that the container must run as a non-root user. If true, the Kubelet will validate the image at runtime to ensure that it does not run as UID 0 (root) and fail to start the container if it does. If unset or false, no such validation will be performed. May also be set in PodSecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence."

### fn spec.authProxyContainer.container.securityContext.withRunAsUser

```ts
withRunAsUser(runAsUser)
```

"The UID to run the entrypoint of the container process. Defaults to user specified in image metadata if unspecified. May also be set in PodSecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence. Note that this field cannot be set when spec.os.name is windows."

## obj spec.authProxyContainer.container.securityContext.capabilities

"The capabilities to add/drop when running containers. Defaults to the default set of capabilities granted by the container runtime. Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.capabilities.withAdd

```ts
withAdd(add)
```

"Added capabilities"

### fn spec.authProxyContainer.container.securityContext.capabilities.withAddMixin

```ts
withAddMixin(add)
```

"Added capabilities"

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.securityContext.capabilities.withDrop

```ts
withDrop(drop)
```

"Removed capabilities"

### fn spec.authProxyContainer.container.securityContext.capabilities.withDropMixin

```ts
withDropMixin(drop)
```

"Removed capabilities"

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.container.securityContext.seLinuxOptions

"The SELinux context to be applied to the container. If unspecified, the container runtime will allocate a random SELinux context for each container.  May also be set in PodSecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence. Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.seLinuxOptions.withLevel

```ts
withLevel(level)
```

"Level is SELinux level label that applies to the container."

### fn spec.authProxyContainer.container.securityContext.seLinuxOptions.withRole

```ts
withRole(role)
```

"Role is a SELinux role label that applies to the container."

### fn spec.authProxyContainer.container.securityContext.seLinuxOptions.withType

```ts
withType(type)
```

"Type is a SELinux type label that applies to the container."

### fn spec.authProxyContainer.container.securityContext.seLinuxOptions.withUser

```ts
withUser(user)
```

"User is a SELinux user label that applies to the container."

## obj spec.authProxyContainer.container.securityContext.seccompProfile

"The seccomp options to use by this container. If seccomp options are provided at both the pod & container level, the container options override the pod options. Note that this field cannot be set when spec.os.name is windows."

### fn spec.authProxyContainer.container.securityContext.seccompProfile.withLocalhostProfile

```ts
withLocalhostProfile(localhostProfile)
```

"localhostProfile indicates a profile defined in a file on the node should be used. The profile must be preconfigured on the node to work. Must be a descending path, relative to the kubelet's configured seccomp profile location. Must only be set if type is \"Localhost\"."

### fn spec.authProxyContainer.container.securityContext.seccompProfile.withType

```ts
withType(type)
```

"type indicates which kind of seccomp profile will be applied. Valid options are: \n Localhost - a profile defined in a file on the node should be used. RuntimeDefault - the container runtime default profile should be used. Unconfined - no profile should be applied."

## obj spec.authProxyContainer.container.securityContext.windowsOptions

"The Windows specific settings applied to all containers. If unspecified, the options from the PodSecurityContext will be used. If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence. Note that this field cannot be set when spec.os.name is linux."

### fn spec.authProxyContainer.container.securityContext.windowsOptions.withGmsaCredentialSpec

```ts
withGmsaCredentialSpec(gmsaCredentialSpec)
```

"GMSACredentialSpec is where the GMSA admission webhook (https://github.com/kubernetes-sigs/windows-gmsa) inlines the contents of the GMSA credential spec named by the GMSACredentialSpecName field."

### fn spec.authProxyContainer.container.securityContext.windowsOptions.withGmsaCredentialSpecName

```ts
withGmsaCredentialSpecName(gmsaCredentialSpecName)
```

"GMSACredentialSpecName is the name of the GMSA credential spec to use."

### fn spec.authProxyContainer.container.securityContext.windowsOptions.withHostProcess

```ts
withHostProcess(hostProcess)
```

"HostProcess determines if a container should be run as a 'Host Process' container. This field is alpha-level and will only be honored by components that enable the WindowsHostProcessContainers feature flag. Setting this field without the feature flag will result in errors when validating the Pod. All of a Pod's containers must have the same effective HostProcess value (it is not allowed to have a mix of HostProcess containers and non-HostProcess containers).  In addition, if HostProcess is true then HostNetwork must also be set to true."

### fn spec.authProxyContainer.container.securityContext.windowsOptions.withRunAsUserName

```ts
withRunAsUserName(runAsUserName)
```

"The UserName in Windows to run the entrypoint of the container process. Defaults to the user specified in image metadata if unspecified. May also be set in PodSecurityContext. If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence."

## obj spec.authProxyContainer.container.startupProbe

"StartupProbe indicates that the Pod has successfully initialized. If specified, no other probes are executed until this completes successfully. If this probe fails, the Pod will be restarted, just as if the livenessProbe failed. This can be used to provide different probe parameters at the beginning of a Pod's lifecycle, when it might take a long time to load data or warm a cache, than during steady-state operation. This cannot be updated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

### fn spec.authProxyContainer.container.startupProbe.withFailureThreshold

```ts
withFailureThreshold(failureThreshold)
```

"Minimum consecutive failures for the probe to be considered failed after having succeeded. Defaults to 3. Minimum value is 1."

### fn spec.authProxyContainer.container.startupProbe.withInitialDelaySeconds

```ts
withInitialDelaySeconds(initialDelaySeconds)
```

"Number of seconds after the container has started before liveness probes are initiated. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

### fn spec.authProxyContainer.container.startupProbe.withPeriodSeconds

```ts
withPeriodSeconds(periodSeconds)
```

"How often (in seconds) to perform the probe. Default to 10 seconds. Minimum value is 1."

### fn spec.authProxyContainer.container.startupProbe.withSuccessThreshold

```ts
withSuccessThreshold(successThreshold)
```

"Minimum consecutive successes for the probe to be considered successful after having failed. Defaults to 1. Must be 1 for liveness and startup. Minimum value is 1."

### fn spec.authProxyContainer.container.startupProbe.withTerminationGracePeriodSeconds

```ts
withTerminationGracePeriodSeconds(terminationGracePeriodSeconds)
```

"Optional duration in seconds the pod needs to terminate gracefully upon probe failure. The grace period is the duration in seconds after the processes running in the pod are sent a termination signal and the time when the processes are forcibly halted with a kill signal. Set this value longer than the expected cleanup time for your process. If this value is nil, the pod's terminationGracePeriodSeconds will be used. Otherwise, this value overrides the value provided by the pod spec. Value must be non-negative integer. The value zero indicates stop immediately via the kill signal (no opportunity to shut down). This is a beta field and requires enabling ProbeTerminationGracePeriod feature gate. Minimum value is 1. spec.terminationGracePeriodSeconds is used if unset."

### fn spec.authProxyContainer.container.startupProbe.withTimeoutSeconds

```ts
withTimeoutSeconds(timeoutSeconds)
```

"Number of seconds after which the probe times out. Defaults to 1 second. Minimum value is 1. More info: https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#container-probes"

## obj spec.authProxyContainer.container.startupProbe.exec

"Exec specifies the action to take."

### fn spec.authProxyContainer.container.startupProbe.exec.withCommand

```ts
withCommand(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

### fn spec.authProxyContainer.container.startupProbe.exec.withCommandMixin

```ts
withCommandMixin(command)
```

"Command is the command line to execute inside the container, the working directory for the command  is root ('/') in the container's filesystem. The command is simply exec'd, it is not run inside a shell, so traditional shell instructions ('|', etc) won't work. To use a shell, you need to explicitly call out to that shell. Exit status of 0 is treated as live/healthy and non-zero is unhealthy."

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.container.startupProbe.grpc

"GRPC specifies an action involving a GRPC port. This is a beta field and requires enabling GRPCContainerProbe feature gate."

### fn spec.authProxyContainer.container.startupProbe.grpc.withPort

```ts
withPort(port)
```

"Port number of the gRPC service. Number must be in the range 1 to 65535."

### fn spec.authProxyContainer.container.startupProbe.grpc.withService

```ts
withService(service)
```

"Service is the name of the service to place in the gRPC HealthCheckRequest (see https://github.com/grpc/grpc/blob/master/doc/health-checking.md). \n If this is not specified, the default behavior is defined by gRPC."

## obj spec.authProxyContainer.container.startupProbe.httpGet

"HTTPGet specifies the http request to perform."

### fn spec.authProxyContainer.container.startupProbe.httpGet.withHost

```ts
withHost(host)
```

"Host name to connect to, defaults to the pod IP. You probably want to set \"Host\" in httpHeaders instead."

### fn spec.authProxyContainer.container.startupProbe.httpGet.withHttpHeaders

```ts
withHttpHeaders(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.startupProbe.httpGet.withHttpHeadersMixin

```ts
withHttpHeadersMixin(httpHeaders)
```

"Custom headers to set in the request. HTTP allows repeated headers."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.container.startupProbe.httpGet.withPath

```ts
withPath(path)
```

"Path to access on the HTTP server."

### fn spec.authProxyContainer.container.startupProbe.httpGet.withPort

```ts
withPort(port)
```

"Name or number of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

### fn spec.authProxyContainer.container.startupProbe.httpGet.withScheme

```ts
withScheme(scheme)
```

"Scheme to use for connecting to the host. Defaults to HTTP."

## obj spec.authProxyContainer.container.startupProbe.httpGet.httpHeaders

"Custom headers to set in the request. HTTP allows repeated headers."

### fn spec.authProxyContainer.container.startupProbe.httpGet.httpHeaders.withName

```ts
withName(name)
```

"The header field name"

### fn spec.authProxyContainer.container.startupProbe.httpGet.httpHeaders.withValue

```ts
withValue(value)
```

"The header field value"

## obj spec.authProxyContainer.container.startupProbe.tcpSocket

"TCPSocket specifies an action involving a TCP port."

### fn spec.authProxyContainer.container.startupProbe.tcpSocket.withHost

```ts
withHost(host)
```

"Optional: Host name to connect to, defaults to the pod IP."

### fn spec.authProxyContainer.container.startupProbe.tcpSocket.withPort

```ts
withPort(port)
```

"Number or name of the port to access on the container. Number must be in the range 1 to 65535. Name must be an IANA_SVC_NAME."

## obj spec.authProxyContainer.container.volumeDevices

"volumeDevices is the list of block devices to be used by the container."

### fn spec.authProxyContainer.container.volumeDevices.withDevicePath

```ts
withDevicePath(devicePath)
```

"devicePath is the path inside of the container that the device will be mapped to."

### fn spec.authProxyContainer.container.volumeDevices.withName

```ts
withName(name)
```

"name must match the name of a persistentVolumeClaim in the pod"

## obj spec.authProxyContainer.container.volumeMounts

"Pod volumes to mount into the container's filesystem. Cannot be updated."

### fn spec.authProxyContainer.container.volumeMounts.withMountPath

```ts
withMountPath(mountPath)
```

"Path within the container at which the volume should be mounted.  Must not contain ':'."

### fn spec.authProxyContainer.container.volumeMounts.withMountPropagation

```ts
withMountPropagation(mountPropagation)
```

"mountPropagation determines how mounts are propagated from the host to container and the other way around. When not set, MountPropagationNone is used. This field is beta in 1.10."

### fn spec.authProxyContainer.container.volumeMounts.withName

```ts
withName(name)
```

"This must match the Name of a Volume."

### fn spec.authProxyContainer.container.volumeMounts.withReadOnly

```ts
withReadOnly(readOnly)
```

"Mounted read-only if true, read-write otherwise (false or unspecified). Defaults to false."

### fn spec.authProxyContainer.container.volumeMounts.withSubPath

```ts
withSubPath(subPath)
```

"Path within the volume from which the container's volume should be mounted. Defaults to \"\" (volume's root)."

### fn spec.authProxyContainer.container.volumeMounts.withSubPathExpr

```ts
withSubPathExpr(subPathExpr)
```

"Expanded path within the volume from which the container's volume should be mounted. Behaves similarly to SubPath but environment variable references $(VAR_NAME) are expanded using the container's environment. Defaults to \"\" (volume's root). SubPathExpr and SubPath are mutually exclusive."

## obj spec.authProxyContainer.resources

"Resources specifies the resources required for the proxy pod."

### fn spec.authProxyContainer.resources.withClaims

```ts
withClaims(claims)
```

"Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. \n This is an alpha field and requires enabling the DynamicResourceAllocation feature gate. \n This field is immutable. It can only be set for containers."

### fn spec.authProxyContainer.resources.withClaimsMixin

```ts
withClaimsMixin(claims)
```

"Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. \n This is an alpha field and requires enabling the DynamicResourceAllocation feature gate. \n This field is immutable. It can only be set for containers."

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.resources.withLimits

```ts
withLimits(limits)
```

"Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

### fn spec.authProxyContainer.resources.withLimitsMixin

```ts
withLimitsMixin(limits)
```

"Limits describes the maximum amount of compute resources allowed. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

**Note:** This function appends passed data to existing values

### fn spec.authProxyContainer.resources.withRequests

```ts
withRequests(requests)
```

"Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defined value. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

### fn spec.authProxyContainer.resources.withRequestsMixin

```ts
withRequestsMixin(requests)
```

"Requests describes the minimum amount of compute resources required. If Requests is omitted for a container, it defaults to Limits if that is explicitly specified, otherwise to an implementation-defined value. More info: https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/"

**Note:** This function appends passed data to existing values

## obj spec.authProxyContainer.resources.claims

"Claims lists the names of resources, defined in spec.resourceClaims, that are used by this container. \n This is an alpha field and requires enabling the DynamicResourceAllocation feature gate. \n This field is immutable. It can only be set for containers."

### fn spec.authProxyContainer.resources.claims.withName

```ts
withName(name)
```

"Name must match the name of one entry in pod.spec.resourceClaims of the Pod where this field is used. It makes that resource available inside a container."

## obj spec.authProxyContainer.telemetry

"Telemetry specifies how the proxy should expose telemetry. Optional, by default"

### fn spec.authProxyContainer.telemetry.withDisableMetrics

```ts
withDisableMetrics(disableMetrics)
```

"DisableMetrics disables Cloud Monitoring testintegration (used with telemetryProject) This sets the proxy container's CLI argument `--disable-metrics`"

### fn spec.authProxyContainer.telemetry.withDisableTraces

```ts
withDisableTraces(disableTraces)
```

"DisableTraces disables Cloud Trace testintegration (used with telemetryProject) This sets the proxy container's CLI argument `--disable-traces`"

### fn spec.authProxyContainer.telemetry.withHttpPort

```ts
withHttpPort(httpPort)
```

"HTTPPort the port for Prometheus and health check server. This sets the proxy container's CLI argument `--http-port`"

### fn spec.authProxyContainer.telemetry.withPrometheus

```ts
withPrometheus(prometheus)
```

"Prometheus Enables Prometheus HTTP endpoint /metrics on localhost This sets the proxy container's CLI argument `--prometheus`"

### fn spec.authProxyContainer.telemetry.withPrometheusNamespace

```ts
withPrometheusNamespace(prometheusNamespace)
```

"PrometheusNamespace is used the provided Prometheus namespace for metrics This sets the proxy container's CLI argument `--prometheus-namespace`"

### fn spec.authProxyContainer.telemetry.withQuotaProject

```ts
withQuotaProject(quotaProject)
```

"QuotaProject Specifies the project to use for Cloud SQL Admin API quota tracking. The IAM principal must have the \"serviceusage.services.use\" permission for the given project. See https://cloud.google.com/service-usage/docs/overview and https://cloud.google.com/storage/docs/requester-pays This sets the proxy container's CLI argument `--quota-project`"

### fn spec.authProxyContainer.telemetry.withTelemetryPrefix

```ts
withTelemetryPrefix(telemetryPrefix)
```

"TelemetryPrefix is the prefix for Cloud Monitoring metrics. This sets the proxy container's CLI argument `--telemetry-prefix`"

### fn spec.authProxyContainer.telemetry.withTelemetryProject

```ts
withTelemetryProject(telemetryProject)
```

"TelemetryProject enables Cloud Monitoring and Cloud Trace with the provided project ID. This sets the proxy container's CLI argument `--telemetry-project`"

### fn spec.authProxyContainer.telemetry.withTelemetrySampleRate

```ts
withTelemetrySampleRate(telemetrySampleRate)
```

"TelemetrySampleRate is the Cloud Trace sample rate. A smaller number means more traces. This sets the proxy container's CLI argument `--telemetry-sample-rate`"

## obj spec.instances

"Instances describes the Cloud SQL instances to configure on the proxy container."

### fn spec.instances.withAutoIAMAuthN

```ts
withAutoIAMAuthN(autoIAMAuthN)
```

"AutoIAMAuthN (optional) Enables IAM Authentication for this instance. Default value is false."

### fn spec.instances.withConnectionString

```ts
withConnectionString(connectionString)
```

"ConnectionString is the connection string for the Cloud SQL Instance in the format `project_id:region:instance_name`"

### fn spec.instances.withHostEnvName

```ts
withHostEnvName(hostEnvName)
```

"HostEnvName The name of the environment variable containing this instances tcp hostname Optional, when set this environment variable will be added to all containers in the workload."

### fn spec.instances.withPort

```ts
withPort(port)
```

"Port (optional) sets the tcp port for this instance. If not set, a value will be automatically assigned by the operator and set as an environment variable on all containers in the workload named according to PortEnvName. The operator will choose a port so that it does not conflict with other ports on the workload."

### fn spec.instances.withPortEnvName

```ts
withPortEnvName(portEnvName)
```

"PortEnvName is name of the environment variable containing this instance's tcp port. Optional, when set this environment variable will be added to all containers in the workload."

### fn spec.instances.withPrivateIP

```ts
withPrivateIP(privateIP)
```

"PrivateIP (optional) Enable connection to the Cloud SQL instance's private ip for this instance. Default value is false."

### fn spec.instances.withUnixSocketPath

```ts
withUnixSocketPath(unixSocketPath)
```

"UnixSocketPath is the path to the unix socket where the proxy will listen for connnections. This will be mounted to all containers in the pod."

### fn spec.instances.withUnixSocketPathEnvName

```ts
withUnixSocketPathEnvName(unixSocketPathEnvName)
```

"UnixSocketPathEnvName is the environment variable containing the value of UnixSocketPath."

## obj spec.workloadSelector

"Workload selects the workload where the proxy container will be added."

### fn spec.workloadSelector.withKind

```ts
withKind(kind)
```

"Kind specifies what kind of workload Supported kinds: Deployment, StatefulSet, Pod, ReplicaSet,DaemonSet, Job, CronJob Example: \"Deployment\" \"Deployment.v1\" or \"Deployment.v1.apps\"."

### fn spec.workloadSelector.withName

```ts
withName(name)
```

"Name specifies the name of the resource to select."

## obj spec.workloadSelector.selector

"Selector (optional) selects resources using labels. See \"Label selectors\" in the kubernetes docs https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors"

### fn spec.workloadSelector.selector.withMatchExpressions

```ts
withMatchExpressions(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.workloadSelector.selector.withMatchExpressionsMixin

```ts
withMatchExpressionsMixin(matchExpressions)
```

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

**Note:** This function appends passed data to existing values

### fn spec.workloadSelector.selector.withMatchLabels

```ts
withMatchLabels(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

### fn spec.workloadSelector.selector.withMatchLabelsMixin

```ts
withMatchLabelsMixin(matchLabels)
```

"matchLabels is a map of {key,value} pairs. A single {key,value} in the matchLabels map is equivalent to an element of matchExpressions, whose key field is \"key\", the operator is \"In\", and the values array contains only \"value\". The requirements are ANDed."

**Note:** This function appends passed data to existing values

## obj spec.workloadSelector.selector.matchExpressions

"matchExpressions is a list of label selector requirements. The requirements are ANDed."

### fn spec.workloadSelector.selector.matchExpressions.withKey

```ts
withKey(key)
```

"key is the label key that the selector applies to."

### fn spec.workloadSelector.selector.matchExpressions.withOperator

```ts
withOperator(operator)
```

"operator represents a key's relationship to a set of values. Valid operators are In, NotIn, Exists and DoesNotExist."

### fn spec.workloadSelector.selector.matchExpressions.withValues

```ts
withValues(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

### fn spec.workloadSelector.selector.matchExpressions.withValuesMixin

```ts
withValuesMixin(values)
```

"values is an array of string values. If the operator is In or NotIn, the values array must be non-empty. If the operator is Exists or DoesNotExist, the values array must be empty. This array is replaced during a strategic merge patch."

**Note:** This function appends passed data to existing values