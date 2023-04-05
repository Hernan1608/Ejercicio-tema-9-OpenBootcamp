# Ejercicio-tema-9-OpenBootcamp
Ejercicio tema 9 
public class Persona {
    private int edad;
    private String nombre;
    private String telefono;

    public int getEdad() {
        return edad;
    }

    public void setEdad(int edad) {
        this.edad = edad;
    }

    public String getNombre() {
        return nombre;
    }

    public void setNombre(String nombre) {
        this.nombre = nombre;
    }

    public String getTelefono() {
        return telefono;
    }

    public void setTelefono(String telefono) {
        this.telefono = telefono;
    }
}

public class Cliente extends Persona {
    private double credito;

    public double getCredito() {
        return credito;
    }

    public void setCredito(double credito) {
        this.credito = credito;
    }
}

public class Trabajador extends Persona {
    private double salario;

    public double getSalario() {
        return salario;
    }

    public void setSalario(double salario) {
        this.salario = salario;
    }
}

// En el método main:

public static void main(String[] args) {
    // Crear objeto Cliente
    Cliente cliente = new Cliente();
    cliente.setEdad(35);
    cliente.setNombre("Ana");
    cliente.setTelefono("123456789");
    cliente.setCredito(5000.0);

    System.out.println("Cliente: " + cliente.getNombre());
    System.out.println("Edad: " + cliente.getEdad());
    System.out.println("Teléfono: " + cliente.getTelefono());
    System.out.println("Crédito: " + cliente.getCredito());

    // Crear objeto Trabajador
    Trabajador trabajador = new Trabajador();
    trabajador.setEdad(28);
    trabajador.setNombre("Pedro");
    trabajador.setTelefono("987654321");
    trabajador.setSalario(3000.0);

    System.out.println("Trabajador: " + trabajador.getNombre());
    System.out.println("Edad: " + trabajador.getEdad());
    System.out.println("Teléfono: " + trabajador.getTelefono());
    System.out.println("Salario: " + trabajador.getSalario());
}
