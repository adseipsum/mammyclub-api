#

<img src='https://g.gravizo.com/svg?%40startuml%0Aparticipant%20%22mammyclub%20(CI1.7)%22%20as%20MC%0Aparticipant%20%22Database%22%20as%20DB%0Aparticipant%20%22Event%20Pipe%22%20as%20EP%0Aparticipant%20%22RabbitMQ%22%20as%20RM%0Aparticipant%20%22API%20Gates%20(Symfony%203.4)%22%20as%20API%0Aparticipant%20%22%D0%9C%D0%BE%D0%B9%20%D0%A1%D0%BA%D0%BB%D0%B0%D0%B4%22%20as%20MS%0AMC-%3E%20DB%3A%20query%0Aactivate%20MC%0AMC-%3EDB%3A%20on%20query%20save%20event%20to%20DB%0Adeactivate%20MC%0ADB-%3EEP%3A%20get%20events%0Aactivate%20EP%0AEP--%3E%20RM%3A%20send%20event%20message%0Adeactivate%20EP%0AAPI--%3E%20RM%3A%20subscribe%20event%20message%0Aactivate%20API%0AAPI%20--%3E%20MS%3A%20HTTP%0Adeactivate%20API%0Aactivate%20MS%0AMS%20--%3E%20API%3A%20HTTP%0Adeactivate%20MS%0Aactivate%20API%0AAPI--%3E%20RM%3A%20send%20response%20message%0Adeactivate%20API%0AEP--%3ERM%3A%20subscribe%0Aactivate%20EP%0AEP-%3EDB%3A%20query%0Adeactivate%20EP%0A%40enduml'>
