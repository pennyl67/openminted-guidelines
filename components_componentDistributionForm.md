#### componentDistributionForm

##### Usage

Mandatory

##### Type

closed controlled vocabulary

##### Controlled vocabulary reference and/or values

ms-omtd:componentDistributionMedium: _webService_, _sourceCode_, _executableCode_, _sourceAndExecutableCode, dockerImage_, _galaxyWorkflow_, _workflowFile_

##### Definition/Explanations

The medium/form of the distribution \(e.g. executable code, docker image, workflow etc.\)

**Recommended usage**

* For components registered through Maven, use "executableCode" or "sourceAndExecutableCode"
* For components registered as Docker images, use "dockerImage"
* For web services, use "webService"
* Worfklows created in the OpenMinTeD platform, are automatically assigned the value "galaxyWorkflow".



