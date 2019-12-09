# Sequence of deployment and activation: 
1. Deploy prod-cfp-pdx & prod-las (`passive`) ( ... of which generally the external design deployment or acceptance may fail )
1. Run External Design Deployment **(if failed)**
1. Run Acceptance **(if failed)**
1. Run pre cache **(if failed)**
1. Validate across Teams and wait for PASS from all.
1. Run HTW (Hydra Theme Warming) - https://bamboo.cdk.com/browse/DCP-HTW
1. Activate on prod-cfp-pdx & prod-las

***

Documents for reference:
* https://confluence.cdk.com/pages/viewpage.action?spaceKey=DEV&title=Hydra+Graph+Release+Coordination  
* https://cdkcld.splunkcloud.com/en-GB/app/search/next_gen_error  
* https://cdkcld.splunkcloud.com/en-GB/app/search/next_gen_release_dashboard  
* https://cdk.hostedgraphite.com/31f2825d/grafana/d/000000060/hydra-graph  

***
Release Status: 
 
:unknown: Slide Studio  
:unknown: Editor  
:unknown: Website Calender  
:unknown: Social  
:unknown: Domain Cards  
:unknown: CMS Cards & Consumer Login  
:unknown: GMUI  
:unknown: Agency  
:unknown: CMS  
:unknown: Platform  
:unknown: CUI  
***
