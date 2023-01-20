# Exercise: Smoke Testing
smoke_test:
 docker:
   - image: alpine:latest
 steps:
   - run: apk add --update curl
   - run:
       name: smoke test
       command: |
         URL="https://blog.udacity.com/"
         # Test if website exists
         if curl -s --head ${URL} 
         then
           return 0
         else
           return 1
         fi
