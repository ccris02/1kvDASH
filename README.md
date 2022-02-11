# Grafana Dashboard for 1kv node operator
![1kv](https://user-images.githubusercontent.com/66147586/153630377-a05afd07-4ac0-4a2f-9d20-42c34da1d4e8.PNG)



## 1. Set up a free Grafana Cloud.
https://grafana.com/products/cloud/

You can have up to 10 Dashboards configured for free.
![image](https://user-images.githubusercontent.com/66147586/152935924-901b4bcc-d0b0-4046-bf4e-2dbac6d169da.png)

 
Don’t worry about it, you don’t need the Pro version, everything will work without it.

## 2. Install `JSON API` Plugin
![image](https://user-images.githubusercontent.com/66147586/152935964-16f85d99-b4ce-4806-b270-41143de45346.png)

https://grafana.com/grafana/plugins/marcusolsson-json-datasource/

Plugins – “JSON API” - Version - 1.3.1 Marcus Olsson

Documentation https://marcus.se.net/grafana-json-datasource/

Website https://github.com/marcusolsson/grafana-json-datasource

Grafana >=7.3.0

A data source plugin for loading JSON APIs into Grafana.

It will take few minutes for Plugin to be installed.

## 3. Add Data sources
![image](https://user-images.githubusercontent.com/66147586/152935997-f511c7ea-fcad-43fd-bbc1-c904919b627d.png)

Type in ```JSON```
![image](https://user-images.githubusercontent.com/66147586/152936016-30df5329-3a29-4136-99ab-b34006378610.png)

Make sure to modify the addresses of ksm_1, ksm_2, and dot_1 to display your Validator Stash addresses 
 ![image](https://user-images.githubusercontent.com/66147586/152936047-b3e9aca7-1ac3-4a12-be18-e9cf307beec3.png)

## KUSAMA
- ksm_1_candidate
```https://kusama.w3f.community/candidate/Dq97kmsJXGTciU1eMXZMAp4D41Y9e7kQ4hmFBfZW7YD4CCf```
- ksm_1_erapoint
```https://kusama.w3f.community/erapoints/Dq97kmsJXGTciU1eMXZMAp4D41Y9e7kQ4hmFBfZW7YD4CCf```
- ksm_1_score
```https://kusama.w3f.community/score/Dq97kmsJXGTciU1eMXZMAp4D41Y9e7kQ4hmFBfZW7YD4CCf```
- ksm_2_candidate
```https://kusama.w3f.community/candidate/GnqygxyvFN7npYbMUv6t7avBnLrVB37topoDbhPVnBeeuxa```
- ksm_2_erapoint
```https://kusama.w3f.community/erapoints/GnqygxyvFN7npYbMUv6t7avBnLrVB37topoDbhPVnBeeuxa```
- ksm_2_score
```https://kusama.w3f.community/score/GnqygxyvFN7npYbMUv6t7avBnLrVB37topoDbhPVnBeeuxa```
- ksm_candidates
```https://kusama.w3f.community/candidates```
- ksm_erastats
```https://kusama.w3f.community/erastats```
- ksm_location
```https://kusama.w3f.community/locationstats```

## POLKADOT
- dot_1_candidate
```https://polkadot.w3f.community/candidate/149riLdwAVzXg7Cm88RcXhbuFi3zUgwrGsJSSPjC47PRxHQW```
- dot_1_erapoint
```https://polkadot.w3f.community/erapoints/149riLdwAVzXg7Cm88RcXhbuFi3zUgwrGsJSSPjC47PRxHQW```
- dot_1_score
```https://polkadot.w3f.community/score/149riLdwAVzXg7Cm88RcXhbuFi3zUgwrGsJSSPjC47PRxHQW```
- dot_candidates
```https://polkadot.w3f.community/candidates```
- dot_erastats
```https://polkadot.w3f.community/erastats```
- dot_location
```https://polkadot.w3f.community/locationstats```

You should have 15 data sources
![image](https://user-images.githubusercontent.com/66147586/152936078-a641515b-5e7f-4579-8d37-8e49cf36e1de.png)
![image](https://user-images.githubusercontent.com/66147586/152936101-35681939-70ce-456b-8dcc-01fa3905607e.png)

## 4. Import Dashboard
Match input to data sources from drop down. If you follow the naming convention from step 3 everything should match

![image](https://user-images.githubusercontent.com/66147586/153524297-10c86c06-8a69-4d46-ab51-ce83de056f6a.png)


## 5. Change top of the page links
Top of the page click on the Gear icon > select Links

 ![image](https://user-images.githubusercontent.com/66147586/152936157-38db0c87-b5bb-4acf-a042-573327ed5e54.png)

Modify Polkachu_KSM-1, Polkachu_KSM-2, Polkachu_DOT-1 
To modify link, click on the box with arrow next to the link

 ![image](https://user-images.githubusercontent.com/66147586/152936174-eb7bacdf-e610-4b6f-b440-542d170c9c09.png)

## 6. Dashboard Refresh
Dashboard is configured not to refresh unless you press the refresh button, this can be changed to refresh every 

```(30sec, 1min, 5min, 15min, 30min, 1hr, 2hr, 1day)```

I don't want to waste Will's resources if I don't need to.

