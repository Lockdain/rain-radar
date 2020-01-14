#### Rain radar Lightbend Cloudflow project

Use http://json-generator.com and the following pattern to feed the PrecipationDataHttpIngress
with auto-generated percipation data:
 
` [
   '{{repeat(10, 20)}}',
   {
     timestamp: '{{integer(1574000000000, 1574973230815)}}',
     location: {
       lat: '{{floating(-90.000001, 90)}}',
       lng: '{{floating(-180.000001, 180)}}',
       city: '{{city()}}'
     },
     value: '{{floating(0, 1)}}'
   }
 ]`