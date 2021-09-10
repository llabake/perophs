
- I would go with the feature branching strategy. 
- Developers would create feature branch, after the code is pushed to source control
- The GitlabCI pipeline would detect the new branch, the code is run through the different stages in the pipeline
-- Build
  - The codebase is linted
  - The image is build and scanned for vulnerabilities
-- Test
  - The unit test for the new code is ran
-- Deploy to dev environment
  - The application is deployed to dev environment
-- Deploy to staging environment
  - The application is deployed to staging environment
-- Deploy to production environment
  - The application is deployed to production environment
Any failure in any of these stages would result in the pipeline failing and ci/cd cycle halted at that stage till the relavant fix is made
