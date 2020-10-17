<img src="https://raw.githubusercontent.com/kubernetes/kubernetes/master/logo/logo.png" width="200" alt="Kubernetes" title="Kubernetes">

# Kubernetes

## What is Kubernetes?

The shortest possible definition would be : Kubernetes is a container management technology to manage containerized applications across multiple hosts.

Explaining it further : Kubernetes is a platform which enables us to manage [containerized](#Glossary) applications (workloads, services) that faciliates automation.

Let's take an example.

Suppose you have an application in a container. During production, if this container goes down, you are losing end-users. You need to track these down and bring another container up as soon as possible. This whole thing is systematically done and maintained by Kubernetes.

Kubernetes provides you with a framework to run your application. It then handles failovers of your application, manages scaling and more. It is used widely in [canary deployments](#Glossary). It is portable, extensible and open-source. The open source project is hosted by [Cloud Native Computing Foundation](https://www.cncf.io/).

### Glossary

1. **Container** : A package that contains all of application's dependencies so that the app can run quickly and reliably on all computing environments.

2. **Containerized application** : An application that is in a container. Thus, with this virtualization method, we don't have to launch the entire virtual-machine for each app.

3. **Canary deployment** : It is a pattern for releasing application changes or rolling out releases. The application is first released to a small subset of end-users. The application is tested there. On successful testing, the release is rolled-out for the rest of the user-base.

## Sources

- [Kubernetes - GitHub](https://github.com/kubernetes/kubernetes)
- [Kubernetes - Official Website](https://kubernetes.io/docs/home/)
