- š Hi, Iām @Fady-Aziz7
- š Iām interested in Learning new skills in coding 
- š± Iām currently learning Workflow 
- šļø Iām looking to collaborate on ...
- š« How to reach me fadyness911@gmail.com

<!---
Fady-Aziz7/Fady-Aziz7 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
workflows:
  version: 2
  build-test-and-deploy:
    jobs:
      - build
      - test1:
          requires:
            - build
      - test2:
          requires:
            - test1
      - deploy:
          requires:
            - test2
