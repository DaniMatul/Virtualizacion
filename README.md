# Assessment 06 - Argo CD and GitOps

## Argo CD Access

Argo CD was accessed using the local domain:

`http://argocd.mdma.local`

![Argo CD Login](images/image1.png)

---

## Applications

At first, there were no applications created in Argo CD.

![No Applications](images/image2.png)

After creating `app1` and `app2`, both applications appeared as `Healthy` and `Synced`.

![Applications Synced and Healthy](images/image3.png)

The same status was verified from the terminal.

![Applications Status in Terminal](images/image4.png)

---

## App1 Before the Change

The `app1` application was synchronized correctly.

![App1 Before Change](images/image5.png)

The application status was `Healthy` and `Synced`.

![App1 Synced](images/image6.png)

---

## GitOps Synchronization Test

The number of replicas in `app1` was changed from `1` to `3`.

The change was committed and pushed to GitHub.

Argo CD detected the change and synchronized the cluster automatically.

![App1 with Three Replicas](images/image7.png)

---

## Conclusion

Argo CD was installed and configured successfully.

Two applications were deployed using GitOps, and the change in `app1` was synchronized automatically.