### Deploy integration:

```bash
git clone https://github.com/styblope/cp4aiops-smax-integration-public.git
cd cp4aiops-smax-integration-public

oc create -f bundlemanifest.yaml -n cp4aiops
```

Ensure the deployed BundleManifest is running. Be patient, it takes a few moments to set things up.
```bash
oc get bundlemanifest | grep smax
smax                 Configured
```

### Create test incidents

1. create an Automation to generate test alerts: [createAlert.md](./createAlert.md)
2. configure a Policy to create Incidents and emit then to SMAX: [createPolicy.md](./createPolicy.md)
