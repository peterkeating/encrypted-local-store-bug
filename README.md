# Encrypted Local Store Bug

Sample application demonstrating a bug with the EncryptedLocalStore caused when upgrading from AIR 3.3 to AIR 3.4.

## Submitted Bug

A bug report has been submitted to Adobe's bug tracker and can be found from the link below.

[https://bugbase.adobe.com/index.cfm?event=bug&id=3315763](https://bugbase.adobe.com/index.cfm?event=bug&id=3315763)

## Forum Post

There is a thread on the Adobe forums about the bug that can be found from the link below.

[http://forums.adobe.com/message/4647863#4647863](http://forums.adobe.com/message/4647863#4647863) 

## Download

You can download the installer for the sample application from the [downloads section](https://github.com/peterkeating/encrypted-local-store-bug/downloads).

## Recreating the bug

Run the application with AIR 3.3 (or any versions before), you should see that a value is created in the EncryptedLocalStore. Switch your AIR runtime to 3.4, you will see that once again a value has been created in the EncryptedLocalStore, this occurs because the AIR 3.4 runtime is unable to retrieve that value that was set in the EncryptedLocalStore by the 3.4 runtime. The example application creates a random value, so now switching between the different AIR runtimes means a different value is displayed.

## Expected Result

The values returned from the EncryptedLocalStore by the AIR 3.4 should be the same value that was set while running the application in the AIR 3.3 runtime.

## Solution

Currently isn't one.
