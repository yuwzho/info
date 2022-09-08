1. Visit [Azure Spring Apps Enterprise Offer](https://ms.portal.azure.com/#view/Microsoft_Azure_Marketplace/GalleryItemDetailsBladeNopdl/id/vmware-inc.azure-spring-cloud-vmware-tanzu-2) through Azure Portal
1. Check "Plans + Pricing" tab, make sure you can see the new free plan.
    > If not, you should whitelist your tenant Id in the Marketplace Partner Center
    ![image](https://user-images.githubusercontent.com/14213176/189024542-2d73e4e4-0a17-4a46-8a50-d2b722b121bf.png)

 1. Open the "Cloud Shell" on the portal
 
    ![image](https://user-images.githubusercontent.com/14213176/189025225-26a78aff-749a-4390-8bb3-c205fbf4d5ff.png)

 3. Run command `token=$(az account get-access-token --query accessToken -o tsv);curl -H "Authorization: Bearer ${token}" https://management.azure.com/providers/Microsoft.Marketplace/offers/vmware-inc.azure-spring-cloud-vmware-tanzu-2?api-version=2018-08-01-beta&market=US;`    
 4. Copy the output and send to ASA team.
    ![image](https://user-images.githubusercontent.com/14213176/189024994-0a420ca2-fb86-4366-bdc6-30f591ea2822.png)
