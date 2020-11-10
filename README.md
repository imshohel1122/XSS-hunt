# XSS-hunt



ALL SET NOW MASS HUNT FOR XSS (step by step)
=============================
echo "yourtarget.com" | waybackurls | tee target.txt 
cat target.txt | gf xss | sed 's/=.*/=/' | sed 's/URL: //' | tee targetxss.txt
dalfox file targetxss.txt pipe
