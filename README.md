Deploy integration:
```bash
git clone https://github.com/styblope/cp4aiops-smax-integration-public.git
cd cp4aiops-smax-integration-public

oc create -f bundlemanifest.yaml -n cp4aiops
```

Ensure the deployed BundleManifest is running:
```bash
oc get bundlemanifest | grep smax
ticket-template                 Configured
```
