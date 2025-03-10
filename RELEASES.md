# Release Notes

#### FluentStorage.Azure.Blobs 5.2.2
 - Fix: Upgrade `System.Text.Json` package from v4 to v7

#### FluentStorage 5.2.2
 - Fix: Upgrade `System.Text.Json` package from v4 to v7
 - Fix: Local storage: Handling of `LastModificationTime` and `CreatedTime`
 - Fix: Local storage: `LastAccessTimeUtc` is saved as a Universal sortable string in the Blob properties

#### FluentStorage.SFTP 5.2.3
 - Fix: Various fixes to `ListAsync` path handling
 - Fix: Upgrade `SSH.NET` package from v2016 to v2020

#### FluentStorage.SFTP 5.2.2
 - New: Added support for a root path in the SFTP connection string
 - Fix: `GetBlobsAsync` should return an array with a single null if the file does not exist
 - Fix: `WriteAsync` will create the directory if it does not exist

#### FluentStorage 5.2.1
 - New: Implement `LocalDiskMessenger.StartProcessorAsync`
 - Package: Add Nuget reference to `Newtonsoft.Json 13.0.3`
 - Package: Remove Nuget reference to `Newtonsoft.Json 12.x.x`
 - Package: Remove Nuget reference to `NetBox` and add the required utilities within this library

#### FluentStorage.AWS 5.2.1
 - New: Implement server-side filtering in `AwsS3DirectoryBrowser.ListAsync` by supplying a `FilePrefix` (thanks SRJames)

#### FluentStorage.FTP 5.2.1
 - Fix: Support for the append parameter in FluentFtpBlobStorage (thanks candoumbe)
 - Fix: `IBlobStorage.WriteAsync` will create the directory hierarchy if required (thanks candoumbe)

#### FluentStorage 5.1.1
 - Fix: Implementation of `LocalDiskMessenger.StartProcessorAsync` (issue [#14](https://github.com/robinrodricks/FluentStorage/issues/14))(`netstandard2.1` / `net6.0` and above

#### FluentStorage 5.0.0
 - New: Introducing the FluentStorage set of libraries created from Storage.NET
 - New: Added SFTP provider using [SSH.NET](https://github.com/sshnet/SSH.NET)
 - Fix: FTP provider [FluentFTP](https://github.com/robinrodricks/FluentFTP) updated to v44
 - Fix: AWS Nugets bumped to latest versions as of Jan 2023
 - Fix: All nuget packages now target `netstandard2.0`,`netstandard2.1`,`net50`,`net60`
 - Change: Refactored package structure to simplify naming scheme
 - Change: Refactored entire codebase to simplify code organization
 - New: Documentation wiki created with one page per provider