# Macam-macam authorization KrakenD
1. JWT Validation : memvalidasi token 
2. JWT Signing : men-generate token 
3. OAuth2 Client credentials : melalui OAuth2 krakenD dapat melaukan request ke server authorization sebuah akses token untuk mencapai resource yang terproteksi 

Untuk example filenya https://github.com/devopsfaith/krakend-playground

Endpoint yang perlu diperhatikan :

     /private/auth0: Melindungi dan memvalidasi titik akhir token JWT yang dikeluarkan oleh Auth0
     /private/custom: Melindungi dan memvalidasi titik akhir token JWT kustom yang didapat dari /token.
     /token: Mengenerate token
  
