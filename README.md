# protect.R

## what exactly is protect.R?
So everybody warns me, rightly so, that Protection data is extremely confidential. I agree 100%; GBV is a volatile space, as is Child Protection. PSEA, case management and everything in between, require mine action people and attorneys because human-rights and data protection things easily explode. Do no harm!

Trust me, I really get it. No monkey-business with protection data.

So, what is my job again? I am the Protection IM Specialist. Look, I love the tools that my job gives me until I feel like I invented the damn rainbow with R. Now, I want to paint a few new rainbow-colors with my time and skill...protect.R!  

## protect.R prerequisites

This is a shinyapp done in R. Sorry STATA and SPSS guys; please go away!

protect.R uses the `geocode()` function in the R package `ggmap`. For this geocoding mapping tool to work, you will need to create an account on Google Cloud Platform and generate an API key to Google's Geocoding API. Additionally, you will need to create a file keyring.R and store the register your key for Google's Geocoding API like so:

```{r eval = FALSE}
googleKey <- "your-API-key"
register_google(key = googleKey) #register for ggmap
```

This script will be used server.R