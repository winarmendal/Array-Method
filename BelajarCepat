public class BelajarCepat {

    private int array[];
    private int count;
    private int sizeofarray;

    public BelajarCepat() {
        array = new int[1];
        count = 0;
        sizeofarray = 1;
    }

    public void tambahElement(int a) {
        if (count == sizeofarray) {
            perbesarUkuranArray();
        }
        array[count] = a;
        count++;
    }

    public void perbesarUkuranArray() {
        int temp[] = null;
        if (count == sizeofarray) {
            temp = new int[sizeofarray * 2];
            {
                for (int i = 0; i < sizeofarray; i++) {
                    temp[i] = array[i];
                }
            }
        }
        array = temp;
        sizeofarray = sizeofarray * 2;
    }

    public void perkecilUkuranArray() {
        int temp[];
        if (count > 0) {
            temp = new int[count];
            System.arraycopy(array, 0, temp, 0, count);
            sizeofarray = count;
            array = temp;
        }
    }

    public void hapusElement() {
        if (count > 0) {
            array[count - 1] = 0;
            count--;
        }
    }

    public void hapusElementByIndex(int index) {
        if (count > 0) {
            for (int i = index; i < count - 1; i++) {
                array[i] = array[i + 1];
            }
            array[count - 1] = 0;
            count--;
        }
    }

    public static void main(String[] args) {
        BelajarCepat bc = new BelajarCepat();

        bc.tambahElement(12);
        bc.tambahElement(22);
        bc.tambahElement(35);
        bc.tambahElement(47);
        bc.tambahElement(85);
        bc.tambahElement(26);
        bc.tambahElement(70);
        bc.tambahElement(81);
        bc.tambahElement(96);
        bc.tambahElement(54);
        
        System.out.println("Element-element array:");
        for (int i = 0; i < bc.sizeofarray; i++) {
            System.out.print(bc.array[i] + " ");
        }
        
        System.out.println("\nUkuran array: " + bc.sizeofarray);
        System.out.println("Jumlah element: " + bc.count);
        bc.hapusElement();
        System.out.print("\nElement array setelah element yang terkahir dihapus: ");
        for (int i = 0; i < bc.sizeofarray; i++) {
            System.out.print(bc.array[i] + " ");
        }

        System.out.println("\nUkuran array: " + bc.sizeofarray);
        System.out.println("Jumlah element: " + bc.count);
        bc.hapusElementByIndex(7);
        System.out.print("\nElement array setelah penghapusan element pada index ke 7: ");
        for (int i = 0; i < bc.sizeofarray; i++) {
            System.out.print(bc.array[i] + " ");
        }
        
        System.out.println("\nUkuran array: " + bc.sizeofarray);
        System.out.println("Jumlah element: " + bc.count);
    }
}
