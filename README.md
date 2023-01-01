# assignment
Assignment for Software Engineering Intern



# Google maps API Key : 
AIzaSyCGXLU-744-Zz2CJUsihhdXmvAWL6M7uKs

# Python pesitiontrack
import http.client, urllib.parse

conn = http.client.HTTPConnection('api.positionstack.com')

params = urllib.parse.urlencode({
    'access_key': 'e96c6aec4e1871e95e9ecbd6bc9a3e1f',
    'query': 'Copacabana',
    'region': 'Rio de Janeiro',
    'limit': 1,
    })

conn.request('GET', '/v1/forward?{}'.format(params))

res = conn.getresponse()
data = res.read()

print(data.decode('utf-8'))


# Nada Suwan
