# zeus
A collection of CLI commands for web application debugging.

Commands

#1 Check if request is handled by Fastly.

`curl -svo /dev/null test.pif.today -H "Fastly-Debug: true"`

To that end the above curl request if handled by Fastly will emit some extra Fastly debug headers.

#2 Check CAA record.

`host -t caa domain.com`

#3 Check the cname.

`host -t cname domain.com`

#4 Check the A record.

`host -t a domain.com`

#5 Check the AAAA record.

`host -t aaaa domain.com`

#6 Check the txt record

`host -t txt domain.com`

#7 Check the mx record.

`host -t mx domain.com`

#8 Check the NS record.

`host -t ns domain.com`

#9 Check SOA (start of Authority ) record.

`host -t soa domain.com`

#10 Check PTR record.

`host -t ptr domain.com`
