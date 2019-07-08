# ![LOGO](logo.png) AWS Import/Export **flow**ground Connector

## Description

A generated **flow**ground connector for the AWS Import/Export API (version 2010-06-01).

Generated from: https://api.apis.guru/v2/specs/amazonaws.com/importexport/2010-06-01/swagger.json<br/>
Generated at: 2019-07-08T14:35:39+03:00

## API Description

<fullname>AWS Import/Export Service</fullname> AWS Import/Export accelerates transferring large amounts of data between the AWS cloud and portable storage devices that you mail to us. AWS Import/Export transfers data directly onto and off of your storage devices using Amazon's high-speed internal network and bypassing the Internet. For large data sets, AWS Import/Export is often faster than Internet transfer and more cost effective than upgrading your connectivity.<br/>

## Authorization

Supported authorization schemes:
- API Key
## Actions

### CancelJob
> This operation cancels a specified job. Only the job owner can cancel it. The operation fails if the job has already started or is complete.<br/>

#### Input Parameters
* `Operation` - _required_
    Possible values: CancelJob.
* `Action` - _required_
* `SignatureMethod` - _required_
* `SignatureVersion` - _required_
* `Timestamp` - _required_
* `Version` - _required_
* `Signature` - _required_

### CreateJob
> This operation initiates the process of scheduling an upload or download of your data. You include in the request a manifest that describes the data transfer specifics. The response to the request includes a job ID, which you can use in other operations, a signature that you use to identify your storage device, and the address where you should ship your storage device.<br/>

#### Input Parameters
* `Operation` - _required_
    Possible values: CreateJob.
* `Action` - _required_
* `SignatureMethod` - _required_
* `SignatureVersion` - _required_
* `Timestamp` - _required_
* `Version` - _required_
* `Signature` - _required_

### GetShippingLabel
> This operation generates a pre-paid UPS shipping label that you will use to ship your device to AWS for processing.<br/>

#### Input Parameters
* `Operation` - _required_
    Possible values: GetShippingLabel.
* `Action` - _required_
* `SignatureMethod` - _required_
* `SignatureVersion` - _required_
* `Timestamp` - _required_
* `Version` - _required_
* `Signature` - _required_

### GetStatus
> This operation returns information about a job, including where the job is in the processing pipeline, the status of the results, and the signature value associated with the job. You can only return information about jobs you own.<br/>

#### Input Parameters
* `Operation` - _required_
    Possible values: GetStatus.
* `Action` - _required_
* `SignatureMethod` - _required_
* `SignatureVersion` - _required_
* `Timestamp` - _required_
* `Version` - _required_
* `Signature` - _required_

### ListJobs
> This operation returns the jobs associated with the requester. AWS Import/Export lists the jobs in reverse chronological order based on the date of creation. For example if Job Test1 was created 2009Dec30 and Test2 was created 2010Feb05, the ListJobs operation would return Test2 followed by Test1.<br/>

#### Input Parameters
* `MaxJobs` - _optional_ - Pagination limit<br/>
* `Marker` - _optional_ - Pagination token<br/>
* `Operation` - _required_
    Possible values: ListJobs.
* `SignatureVersion` - _required_
* `Timestamp` - _required_
* `Version` - _required_
* `Signature` - _required_

### UpdateJob
> You use this operation to change the parameters specified in the original manifest file by supplying a new manifest file. The manifest file attached to this request replaces the original manifest file. You can only use the operation after a CreateJob request but before the data transfer starts and you can only use it on jobs you own.<br/>

#### Input Parameters
* `Operation` - _required_
    Possible values: UpdateJob.
* `Action` - _required_
* `SignatureMethod` - _required_
* `SignatureVersion` - _required_
* `Timestamp` - _required_
* `Version` - _required_
* `Signature` - _required_

## License

**flow**ground :- Telekom iPaaS / amazonaws-com-importexport-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
