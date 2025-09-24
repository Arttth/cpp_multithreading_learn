✅ Roadmap по многопоточности в C++
📌 Фаза 1. База (1–1.5 мес.)

- [ ] Изучить различия: процессы vs потоки, race condition, deadlock.

 - [ ] Освоить std::thread, std::mutex, std::condition_variable.

 - [ ] 📚 Прочитать главы 1–4 из C++ Concurrency in Action.

 - [ ] 📚 Почитать cppreference (раздел Concurrency).

 - [ ] 🛠 Попробовать ThreadSanitizer / Helgrind.

Проекты:

 - [ ] Ping-Pong (два потока печатают по очереди).

 - [ ] Producer–Consumer (mutex + queue).

 - [ ] Счётчик с гонками → исправить через mutex.

📌 Фаза 2. C++11/14/17 Concurrency (1.5–2 мес.)

 - [ ] Изучить std::future, std::promise, std::async.

 - [ ] Разобраться с RAII-locks (std::lock_guard, std::unique_lock).

 - [ ] Начать работу с std::atomic.

 - [ ] 📚 Прочитать главы 5–7 из C++ Concurrency in Action.

 - [ ] 🛠 Google Benchmark для измерения производительности.

- [ ] Проекты:

 - [ ] ThreadPool (базовый).

 - [ ] Async calculator (future/promise).

 - [ ] Thread-safe Queue.

📌 Фаза 3. Memory Model и производительность (2 мес.)

 - [ ] Изучить memory order (relaxed, acquire, release, seq_cst).

 - [ ] Разобраться с false sharing и cache line alignment.

 - [ ] Ознакомиться с NUMA.

 - [ ] 📚 Прочитать статьи Jeff Preshing про memory ordering.

 - [ ] 📺 Посмотреть Herb Sutter — atomic<> Weapons.

 - [ ] 🛠 Использовать perf / Intel VTune для анализа кода.

Проекты:

 - [ ] Lock-free счётчик (std::atomic).

 - [ ] Тест reorderings (эксперименты с memory_order).

 - [ ] False Sharing demo (alignas).

📌 Фаза 4. Паттерны и архитектура (1.5 мес.)

 - [ ] Изучить паттерны: producer–consumer, reader–writer, fork–join, actor model.

 - [ ] Разобраться с thread pools (включая work stealing).

 - [ ] 📚 Прочитать Patterns for Parallel Programming.

 - [ ] 🛠 Освоить Intel TBB (oneTBB).

 - [ ] 🛠 Boost.Thread, Boost.Asio.

Проекты:

 - [ ] Logging system (отдельный поток пишет в файл).

 - [ ] Echo-server (TCP) с пулом потоков.

 - [ ] Мини-Actor system.

📌 Фаза 5. Low-level (1.5 мес.)

 - [ ] Изучить POSIX Threads (pthreads).

 - [ ] Ознакомиться с WinAPI threads (по необходимости).

 - [ ] Разобраться с futex (Linux).

 - [ ] Изучить shared memory (mmap, shm_open).

 - [ ] 📚 Прочитать Stevens — Advanced Programming in the UNIX Environment.

 - [ ] 📚 Love — Linux System Programming.

 - [ ] 🛠 Использовать strace, perf.

Проекты:

 - [ ] Producer–Consumer на pthreads.

 - [ ] Shared-memory chat.

 - [ ] Мини-runtime для потоков через clone.

📌 Фаза 6. Advanced (2–3 мес.)

 - [ ] Изучить lock-free структуры данных (очереди, hash tables).

 - [ ] Освоить Hazard pointers и RCU.

 - [ ] Разобраться с fibers и cooperative multitasking.

 - [ ] Изучить корутины C++20 (co_await, co_return).

 - [ ] 📚 Vyukov (1024cores.net) — lock-free algorithms.

 - [ ] 📚 Preshing — Lock-Free Programming.

 - [ ] 🛠 Folly, libcds, Concurrency Kit, Seastar, HPX.

Проекты:

 - [ ] Michael–Scott Queue (lock-free MPMC queue).

 RCU demo (словарь с одновременным чтением/обновлением).

 Mini-Actor runtime (как Erlang, но на C++).

 Coroutines + ThreadPool (awaitable задачи).

 📌 Доп. Фаза . Advanced (2–3 мес.)
 
 - [ ] Тесты, стресс тесты
  
 - [ ] Метрики успеха (кол-во операций и тп.)
