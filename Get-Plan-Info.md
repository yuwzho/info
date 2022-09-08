1. Visit [Azure Spring Apps Enterprise Offer](https://ms.portal.azure.com/#view/Microsoft_Azure_Marketplace/GalleryItemDetailsBladeNopdl/id/vmware-inc.azure-spring-cloud-vmware-tanzu-2) through Azure Portal
1. Check "Plans + Pricing" tab, make sure you can see the new free plan.
    > If not, you should whitelist your tenant Id in the Marketplace Partner Center
    
 1. Open the "Cloud Shell" on the portal
 1. Run command `token=$(az account get-access-token --query accessToken -o tsv);curl -H "Authorization: Bearer ${token}" https://management.azure.com/providers/Microsoft.Marketplace/offers/vmware-inc.azure-spring-cloud-vmware-tanzu-2?api-version=2018-08-01-beta&market=US;`    
 1. Copy the output and send to ASA team.
