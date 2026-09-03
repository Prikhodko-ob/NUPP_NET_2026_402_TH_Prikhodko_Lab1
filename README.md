class Bus : Vehicle {
      public Guid Id { get; set; }
      public int capacity { get; set; }
      public string Root { get; set; }
      public double FuelConsumption { get; set; }
      ...
}

class Ticket {
      public Guid Id { get; set; }
      public double Price { get; set; }
      public string SerialNumber { get; set; }
      ...
}
class Bus : Vehicle {
      // конструктор
public BUS() {}
public interface ICrudService<T> {
	public void Create(T element);
	public T Read(Guid id);
	public IEnumerable<T> ReadAll();
	public void Update(T element);
	public void Remove(T element);
