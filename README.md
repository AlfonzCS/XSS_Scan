# XSS_Scan

# Uso:
```
python3 XSS.py http://testphp.vulnweb.com/search.php?test=query
```
# Output:
```
═╗ ╦╔═╗╔═╗
╔╩╦╝╚═╗╚═╗─────────────+
╩ ╚═╚═╝╚═╝────AlfonzCS |

[+] Detected 1 forms on http://testphp.vulnweb.com/search.php?test=query.
[+] XSS Detected on http://testphp.vulnweb.com/search.php?test=query
[*] Form details:
{'action': 'search.php?test=query',
 'inputs': [{'name': 'searchFor',
             'type': 'text',
             'value': "<Script>alert('hi')</scripT>"},
            {'name': 'goButton', 'type': 'submit'}],
 'method': 'post'}
True
```
