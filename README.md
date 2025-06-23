# ter-homeworks-05

# Задание 1

## tflint

src

![Снимок экрана 2025-06-23 180629](https://github.com/user-attachments/assets/d5905584-ff71-48e4-a95f-e01e80fadf9e)

_Ошибки: Не используемые переменные. Отсутствие ограничения на версию провайдера._

passwords

![Снимок экрана 2025-06-23 180647](https://github.com/user-attachments/assets/e08bf0c9-b292-4cb8-8384-4af4c55f28b9)

_Ошибки: Отсутствие ограничения на версию провайдера._

vms

![Снимок экрана 2025-06-23 180502](https://github.com/user-attachments/assets/c06fcc30-94e0-47ed-999f-965d15a179f5)

_Ошибки: Требование указывать хеш коммита, а не имя ветки (main).Не используемые переменные. Отсутствие ограничения на версию провайдера._

## checkov

docker pull bridgecrew/checkov

docker run --rm --tty --volume $(pwd):/tf --workdir /tf bridgecrew/checkov --download-external-modules true --directory /tf

vms

![Снимок экрана 2025-06-23 175925](https://github.com/user-attachments/assets/af9796ac-8a18-4591-a46b-cb5ec75ced93)

![Снимок экрана 2025-06-23 175938](https://github.com/user-attachments/assets/e1340053-a272-4993-aa44-1f995b06db21)

![Снимок экрана 2025-06-23 171100](https://github.com/user-attachments/assets/358da493-8229-44d5-9246-957f5e53fb54)

_Ошибки: Требование указывать хеш коммита, а не имя ветки (main).Не используемые переменные. Отсутствие ограничения на версию провайдера._

- обнаружена ВМ без назначенной группы безопасности на сетевом интерфейсе. (ingress, egress)
- ВМ имеет публичный IP-адрес, что не соответствует рекомендациям безопасности. (типа надо NAT)
- требование указывать хеш коммита или тег, а не имя ветки (main).

passwords, src  

_Ошибки: Не выявлены._

![Снимок экрана 2025-06-23 175740](https://github.com/user-attachments/assets/e026675b-cd35-46fd-8d9b-1c5e5d8c0cd0)

![Снимок экрана 2025-06-23 175837](https://github.com/user-attachments/assets/a3e844af-3631-46a6-83fb-d3ec2886dbf6)




