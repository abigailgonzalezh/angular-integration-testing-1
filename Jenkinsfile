node {stage ( ’ Checkout ’) { checkout scm } stage ( ’ Build ’) { docker 
. image ( ’ trion /ng−cli ’ ) . inside { sh ’npm i n s t a l l ’ sh ’ng 
build −−progress f a l s e −−prod −−aot ’ sh ’ tar −cvzf dist . tar . gz 
−−strip−components=1 dist ’ } archive ’ dist . tar . gz ’ } stage ( ’ 
Test ’) { docker . image ( ’ trion /ng−cli−karma ’ ) . inside { sh ’ng 
test −−progress f a l s e −−watch false ’ } } }
