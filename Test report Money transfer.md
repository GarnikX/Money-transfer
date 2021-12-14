14.12.21-14.12.21 было проведено автоматизированное тестирование приложения Money transfer.
На тестирование затрачено: 1 час
В результате автоматизированного тестирования, в среде разработки IntelliJ IDEA Community Edition, с использованием указанных входных данных, выявлены следующие дефекты:
При сложении сумм баланса счета клиента (costumer_account) и денежного перевода (money_transfer) отображается сумма неравная ожидаемой.

Скрин IDEA:
<Money_transfer>
Данные:
<Входные данные https://github.com/netology-code/javaqa-homeworks/blob/master/intro/MERGED.md#:~:text=%D1%82%D0%B5%D0%BA%D1%83%D1%89%D0%B8%D0%B9%20%D0%B1%D0%B0%D0%BB%D0%B0%D0%BD%D1%81%20%D1%81%D1%87%D1%91%D1%82%D0%B0,%D0%B7%D0%BD%D0%B0%D1%87%D0%B5%D0%BD%D0%B8%D1%8F%20%2D%20%D1%82%D0%B8%D0%BF%20int>
Базовое приложение:
public class Main {
    public static void main(String[] args) {
        int costumer_account = 2_000_000_000;
        int money_transfer = 500_000_000;
        int total = costumer_account + money_transfer;
        System.out.println(total);
    }
}

Тестирование производилось в следующем окружении:
Устройство: Ноутбук ASUS X53S Intel Core i7 2.2 ГГц, RAM 4 ГБ, HDD 750 ГБ, GeForce GT 540M
OC: Win7 HB 64
Версия Java 11.0.13

