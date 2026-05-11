Lab Manual 2: Django Microservices Deployment Using Docker Compose

Lab Questions

How does Django support microservices development?

Django supports microservices through its modular design, allowing developers to create small, focused services (like our user_service and product_service). Its built-in support for REST frameworks, environment variables, and database abstraction makes it easy to build autonomous units that communicate over standard protocols like HTTP/JSON.

What advantages do containers provide for Django deployment?

Containers provide environment consistency, ensuring the Django app runs exactly the same in development as it does in production. They also simplify dependency management by bundling the specific Python version and library requirements into a single image, and allow for easy horizontal scaling by spinning up multiple container instances.

How would you enable service-to-service communication?

Service-to-service communication is typically enabled via REST APIs using libraries like requests or httpx. In a Docker Compose environment, services can reach each other using their service names as hostnames (e.g., http://user-service:8000/) thanks to the internal virtual network created by Compose.

How can this setup be scaled using Kubernetes?

This setup can be scaled in Kubernetes by converting the Docker Compose services into Deployments and Services. Kubernetes can then automatically manage "Replicas" of each Django container, handle load balancing between them, and perform self-healing if a container crashes, ensuring high availability for the microservices.


<img width="1919" height="1029" alt="{90C7F201-C952-4419-ABA4-5F4A40CCFFD1}" src="https://github.com/user-attachments/assets/b97bf012-ad63-4812-83a6-86f9741f2050" />



<img width="1919" height="1039" alt="{803E6688-9992-4DD1-8D01-D37895A31F2B}" src="https://github.com/user-attachments/assets/f040b47e-4ce3-4078-87ff-040013712435" />
