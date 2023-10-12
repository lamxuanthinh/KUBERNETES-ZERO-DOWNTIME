# Kubernetes Rolling Update Deployment

## Overview

This project demonstrates how to achieve zero downtime deployment in Kubernetes by utilizing rolling updates. Zero downtime deployments are crucial for ensuring the high availability and reliability of your applications. By following the instructions in this README, you can effectively update your applications running in a Kubernetes cluster without causing service interruptions.

## Prerequisites

Before getting started with this project, make sure you have the following prerequisites:

- [Kubernetes Cluster](https://kubernetes.io/docs/setup/)
- `kubectl` command-line tool configured to connect to your cluster
- Basic knowledge of Kubernetes concepts, such as Deployments and Pods

## Usage

Follow these steps to perform a rolling update of a Kubernetes Deployment:

1. **Clone this Repository**

   ```bash
   git clone https://github.com/yourusername/kubernetes-rolling-update-deployment.git
   ```

2. **Navigate to the Project Directory**

   ```bash
   cd kubernetes-rolling-update-deployment
   ```

3. **Edit the Deployment YAML**

   Modify the `deployment.yaml` file to make the necessary changes to your application. Update the container image, environment variables, or any other parameters as needed.

4. **Apply the Deployment Changes**

   Apply the updated Deployment to your Kubernetes cluster using the `kubectl` command:

   ```bash
   kubectl apply -f deployment.yaml
   ```

5. **Monitor the Rolling Update**

   You can monitor the rolling update by checking the status of the Deployment:

   ```bash
   kubectl get deployments
   ```

   This will show you the progress of the update, ensuring that it is performed in a rolling manner, without any downtime for your application.

6. **Verify the Application**

   Once the update is complete, make sure to verify that your application is running as expected. Test your application and ensure there are no issues.

## Contributing

We welcome contributions from the community. If you have any improvements, bug fixes, or new features to suggest, please open an issue or submit a pull request. See our [Contribution Guidelines](CONTRIBUTING.md) for more details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

We'd like to thank the Kubernetes community for their excellent documentation and resources that helped us put this project together.

## Contact

If you have any questions or need further assistance, feel free to contact us at [thinhlam749@gmail.com](thinhlam749@gmail.com).

---

Happy Deploying!
