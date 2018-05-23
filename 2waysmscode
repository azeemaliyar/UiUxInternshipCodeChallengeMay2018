from AfricasTalkingGateway import AfricasTalkingGateway,AfricasTalkingGatewayException

username = "username"
api_key = "apikey"

number = "254XXXXXXXX"

message = "I'm a lumberjack and it's ok, I sleep all night and I work all day"

gateway = AfricasTalkingGateway(username, api_key)

sender_code = "preconfigured_key"

try:

    results = gateway.sendMessage(number, message, sender_code)

    for r in results:
        print('number=%s;status=%s;messageId=%s;cost=%s' % (r['number'],
                                                            r['status'],
                                                            r['messageId'],
                                                            r['cost']))

except AfricasTalkingGatewayException. e:

    print('Encountered an error while sending: %s' % str(e))
