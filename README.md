# nuxeo-automation-operation-suggestuser-improved
===

## About this module

This module overrides the `UserGroup.Suggestion` which will improve the behaviour of the {{Single user suggestion}} widget when the attribute {{Group id restriction}} is specified.

## Why this module

In the default implementation the `UserGroup.Suggestion` operation only returns the users member of the {{Group id restriction}} group. In the new implementation users of sub-groups will also be returned.

## Building 

        mvn clean install

## Using

The bundle will replace the default `UserGroup.Suggestion` operation, so all you have to do is:

 - to copy the bundle in `nxserver/plugins` or `nxserver/bundles`
 - restart the server

After restart, the `UserGroup.Suggestion` operation will use the new implementation.


