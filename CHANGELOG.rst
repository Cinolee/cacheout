Changelog
=========


v0.7.0 (2018-02-22)
-------------------

- Changed default cache ``maxsize`` from ``300`` to ``256``. (**breaking change**)
- Add ``Cache.memoize()`` decorator.
- Add standalone memoization decorators:

  - ``memoize``
  - ``fifo_memoize``
  - ``lfu_memoize``
  - ``lifo_memoize``
  - ``lru_memoize``
  - ``mru_memoize``
  - ``rr_memoize``


v0.6.0 (2018-02-05)
-------------------

- Add ``LIFOCache``
- Add ``FIFOCache`` as an alias of ``Cache``.


v0.5.0 (2018-02-04)
-------------------

- Add ``LFUCache``
- Delete expired items before popping an item in ``Cache.popitem()``.


v0.4.0 (2018-02-02)
-------------------

- Add ``MRUCache``
- Add ``RRCache``
- Add ``Cache.popitem()``.
- Rename ``Cache.expirations()`` to ``Cache.expire_times()``. (**breaking change**)
- Rename ``Cache.count()`` to ``Cache.size()``. (**breaking change**)
- Remove ``minimum`` arguement from ``Cache.evict()``. (**breaking change**)


v0.3.0 (2018-01-31)
-------------------

- Add ``LRUCache``.
- Add ``CacheManager.__repr__()``.
- Make threading lock usage in ``Cache`` more fine-grained and eliminate redundant locking.
- Fix missing thread-safety in ``Cache.__len__()`` and ``Cache.__contains__()``.


v0.2.0 (2018-01-30)
-------------------

- Rename ``Cache.setup()`` to ``Cache.configure()``. (**breaking change**)
- Add ``CacheManager`` class.


v0.1.0 (2018-01-28)
-------------------

- Add ``Cache`` class.
