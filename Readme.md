  test:
    docker:
      - image: cimg/node: 14.13.0
    steps:
      - checkout
      - run:
        name: install dependencies
        command: npm install
    
      - run:
        name: run tests
        command:  npm run tests
        
