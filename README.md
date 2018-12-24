# connect-github
couchbase-fs-connect-fs Allows you to connect and use a local filesystem as filestorage


## How it works?
it creates meta-key's for a filesystem and stores them with a hostname and connect attribute
to use it for example to catalog your localfilesystem it would be enought to store this meta

#### Importent infos about local
using localhost and local means always local to your connected couchbase-fs-daemon
for security reason this is not allowed normaly but usefull for running small private deployments in cloud setups this should never be used! and also not in multiuser environemtns

```js
meta: {
  hostname: 'localhost' // can be local but then this meta key will error on remote machines so its not as scale able
  protocol: 'local' // ssh, ftp, smb, ntfs , glusterfs ........
}
```

## Supported Protocols are 
- 
