# Virtual Machine

They are scalable compute resources. Azure allows us to choose the size of RAM, CPU power and disk resources, also the number of virtual machines we want to start at the same time. You can programme to start a high number of virtual machines to support your operation during the day and stop all of them or maintain only a minimal number during the night, where a small amount of usage is needed.

We get to consume the operating system along with the VM. So, whenever we choose Linux or Windows, is up to us to install our apps and maintain the OS updated.

## Why would we choose Virtual Machines?

We need to choose Virtual Machines if we need/want control over the operating system. The itens above will be our responsable:

- Patching;
- Version control (of the system and other apps);
- Intrumentation (middlewares);
- Security/Compliance.

## Components

### Images (Azure Marketplace Images)

A collection of prepackaged applications, platforms or services provided by Microsoft and/or third parties.

We can choose between:

- Operating Systens versions (Linux, Windows and versions inside the chosen OS);
- Application infrastructure (Third parties images);
- Custom images (Images created by us or our enterprise).

### Network

It is the network connectivity of the virtual machine with other services/components and to internet.

### Storage

Block storages required for the OS and applications installed by us, the users.

## Creating a Virtual Machine

### Preparation

There are some setup we need to do before creating a Virtual Machine:

- Create a Resource Group

The Virtual Machine will be placed inside the Resource Group.

- Create a Virtual Network

If we don't need to specify the IP Address, for example, Azure will create all this infrastructure for us when we create our Virtual Machine. But if you need to control your network configuration, it's important to create the Virtual Network yourself.

- Choose between Managed Storage or Storage Accounts

Azure will take control of the storage with Managed Storage. Otherwise, we take control with Storage Accounts

### Creation

After the preparation, it's time to create the VM.

- Find a Virtual Machine Image

We need to find an image that suits our needs.

- Give the VM a name

It will make easier for us to find this resource in our inventory.

- Choose the Disk Type

From Premium SSD to standard hard disk drive.

- Define Username and Password

To be able to connect to the VM.

- Select a Subscription

The VM will be linked to the subscription we choose.

- Assigne to a Resource Group

The VM will be linked to the resource group we choose.

- Select the Location or Region

That the VM will be created.

- Select the VM Size

Consists of the CPU, disk and memory.

### Configuring

We need to make final configuration before the submission of the VM to Azure.

- HA and Replication

We can assign the VM to a particular availability zone if it's required.

- Define the Storage type

Like select managed disks.

- Define the Networking

Here we'll assign the VM to the Virtual Network

And if needed: Assign IP (public) and security policies.
