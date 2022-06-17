# azure Application Gateway

# Kubernetes Ingress


# what i am going to do
- Step 1: Creating a new application gateway
- Step 2 : Creating a new application gateway

# Creating a new application gateway

- **Creae a resource group where you have placed a AKS cluster**

```
az group create -n agic -l westus2
```

- **Creae a resource group where you have placed a AKS cluster**

- below command creates a public ip 
```
az network public-ip create -n agic-pip \
    -g agic --allocation-method Static --sku Standard \
    --dns-name "<your unique dns name>"
```

```
az network vnet create -n agic-net -g agic \
    --address-prefix 192.168.0.0/24 --subnet-name agic-subnet \
    --subnet-prefix 192.168.0.0/24

```



# Step 2 : Creating a new application gateway