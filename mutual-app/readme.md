# Installing MCM App

## Steps

1. Download the this project from the git

2. Change the below values according to your cluster in the `/src/mutual-subscription/21-placement.yaml` file

```
  clusterLabels:
    matchExpressions:
      - key: cloud
        operator: In
        values:
        - IBM
```

3. Goto the `install` folder in the command prompt

4. Set the kubetcl context in commmand prompt that points to your mcm hub.

5. Run the below command.

```
sh 01-install.sh
```

The application get installed in the mcm hub.