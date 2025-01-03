aws sqs send-message --queue-url https://sqs.us-east-1.amazonaws.com/476114139866/pendingOrderQueue --message-body "Esto es un mensaje" --region us-east-1

#aws lambda invoke --function-name pizzaApp-dev-sendOrder --region us-east-1 --cli-binary-format raw-in-base64-out --invocation-type Event --payload '{\"orderId\": \"1\",\"pizza\": \"margarita\",\"customerId\": \"abc\"}' response.json