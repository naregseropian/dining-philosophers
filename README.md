### Objective

Develop a simulation of the classic "Dining Philosophers" problem to explore the basics of threading and synchronization in C. The project focuses on creating and managing threads and mutexes to simulate philosophers alternately eating, thinking, and sleeping without encountering race conditions or deadlocks.

### Project Requirements

- **Language**: C
- **Libraries**: pthread, math library (-lm)
- **Functions Used**: memset, printf, malloc, free, write, usleep, gettimeofday, pthread_create, pthread_detach, pthread_join, pthread_mutex_init, pthread_mutex_destroy, pthread_mutex_lock, pthread_mutex_unlock
- **Arguments**: number_of_philosophers, time_to_die, time_to_eat, time_to_sleep, [number_of_times_each_philosopher_must_eat]

### Core Features

- **Multi-threading**: Each philosopher is represented as a separate thread, enabling concurrent execution.
- **Mutexes**: Mutexes are used to manage access to shared resources, preventing race conditions.
- **Simulation Logic**: Philosophers alternate between eating, thinking, and sleeping, ensuring that no philosopher starves while avoiding deadlocks.
- **Time Management**: Precise control over time intervals for each philosopher’s actions, including eating and sleeping durations.

### Implementation

The project simulates philosophers sitting around a table with a bowl of spaghetti. Each philosopher needs two forks (represented by mutexes) to eat. The challenge is to prevent deadlocks and ensure smooth operation even as multiple threads interact with shared resources. Proper synchronization is achieved using mutexes to lock and unlock access to forks.
