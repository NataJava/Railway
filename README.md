# Railway
import com.company.Theatre.BuyTicketInTheatre;

public class Main {

    public static void main(String[] args) {

        //Выберите "есть" или "нет" наличие билета
        BuyTicket ticket = new BuyTicket ("");
        ticket.buy("есть");

        System.out.println();

        //Выбор класса вагона в зависимости от суммы
        Railcar lux=new Railcar1(18000);
        lux.goToCar();
        lux.thereIsInCar("диван-кровать");

        System.out.println();

        Railcar2 SC=new Railcar2(8000);
        SC.goToCar();
        SC.thereIsInCar("2 лежачие полки");

        System.out.println();

        Railcar3 compartment=new Railcar3(3000);
        compartment.goToCar();
        compartment.thereIsInCar("4 лежачие полки");

        System.out.println();

        Railcar4 RSCompartment=new Railcar4(2000);
        RSCompartment.goToCar();
        RSCompartment.thereIsInCar("4 лежачие полки");

        System.out.println();

        Railcar5 seating=new Railcar5(1000);
        seating.goToCar();
        seating.thereIsInCar("кресло");

        System.out.println();

        //Прибытие/отправление поезда в зависимости от времени:09.00-прибытие, 19.00-отправление
        Time o_clock= new Time (0);
        o_clock.watchTime(09.00);

        System.out.println();

        //Поиск своего вагона
        Train number=new Train (0);
        number.search(5,5);

        System.out.println();

        //Проверка документов:"есть" или "нет"
        Ticket document=new Ticket ("");
        document.check("есть");

        //Выберите "есть" или "нет" наличие билета
        BuyTicketInTheatre ticket2=new BuyTicketInTheatre();
        ticket2.buy("есть");

    }
}
