# LocalTime
        LocalTime tm=LocalTime.now();
        System.out.println(tm);
        int sayi=0;
        for (int i = 0; i <100000 ; i++) {
            sayi+=i;
        }
        LocalTime tmLoopSonrasi= LocalTime.now();
        System.out.println(tmLoopSonrasi); 
        double nano1=tm.getNano();
        double nano2=tmLoopSonrasi.getNano();
        System.out.println("islem " + (nano2-nano1));
        System.out.println(tm.plusMinutes(1000)); 
