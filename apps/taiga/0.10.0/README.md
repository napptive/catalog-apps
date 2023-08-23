# Taiga - Open source, Agile project management software

**IMPORTANT:** This application requires at least 8GB of RAM and 2 core CPU to operate properly. Make sure you're environment has these requirements.

For persistent storage, you'll be needing around 2 GB of storage for smooth operation with the base variant. You can modify the storage requirements through the application definition during deployment.

Steps - 
1. Select catalog application.
2. Populate Secret and config map accordingly.
3. Deploy the application.
4. Wait for the backgrounds processes (migrations and rabbitmq connections) to setup (around 5 mins)

Extra-step: If you have public regirstration disabled, then you need to create a superuser using python.
To do that follow these steps: 

1. Download playground CLI from here: [Playground](https://docs.napptive.com/cli/installation.html)
2. Open a terminal session and run `export KUBECONFIG=~/.napptive/default/napptive-kubeconfig`
3. List out pods using `kubectl get pods` and find taiga-back pod. (with pattern taiga-back-<namespace>)
4. Run the command `kubectl exec -it taiga-back-<namespace> -- python manage.py createsuperuser`.
5. Enter details accordingly. 
6. Use that credential to login.
 
**NOTE**: If you have your own Domain name configured for TAIGA, then follow this guide:  https://docs.napptive.com/guides/custom_domains.html
