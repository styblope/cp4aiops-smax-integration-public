Deploy integration:
```bash
oc create -f bundlemanifest.yaml -n cp4aiops
```

Ensure the deployed BundleManifest is running:
```bash
oc get bundlemanifest | grep ticket-template
ticket-template                 Configured
```
