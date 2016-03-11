# Azure Multiple NIC 


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Feldanielo%2FAzureMutltipleNic%2Fmaster%2FAzureMutltipleNic%2FTemplates%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Feldanielo%2FAzureMutltipleNic%2Fmaster%2FAzureMutltipleNic%2FTemplates%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>
<p>
This Template is a simpler version of the <a href="https://azure.microsoft.com/en-us/documentation/articles/virtual-network-deploy-multinic-arm-template/">MultiNIC deployment template</a>, requiring only one resource group. 
</p>
Resources created: </br>
1 Resource Group for all resources </br>
1 Storage Account for all .vhds </br>
1 VNet with 2 Subnets(BackSubnet and FrontSubnet) </br>
2 VMs (frontVM1, frontVM2) with ONE NIC each in the Front Subnet</br>
2 VMs (backVM1, backVM2) with TWO NICs each, one in the FrontSubnet(nic1), the other in the BackSubnet(nic2)</br>

Default VM Sizes represent the minimum configuration for each VM due to <a href="https://azure.microsoft.com/en-us/documentation/articles/virtual-machines-size-specs/">NIC restrictions. </a>