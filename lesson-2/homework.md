# Домашнее задание к лекции №2

## Написать аллокатор со стратегией линейного выделения памяти

Класс должен содержать следующие методы
```c++
class Allocator
{
public:
    void makeAllocator(size_t maxSize);
    char* alloc(size_t size);
    void reset();
};
```

При вызове makeAllocator аллоцируется указанный размер, после чего при вызове alloc возвращает указатель на блок запрошенного размера или nullptr, если места недостаточно. После вызова reset аллокатор позволяет использовать свою память снова.
