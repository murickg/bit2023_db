# CAP теорема и СУБД: DragonFly, ScyllaDB, ArenadataDB

## DragonFly
DragonFly позиционирует себя как а modern replacement for Redis and Memcache (https://github.com/dragonflydb/dragonfly). А именно, она является более ускоренной версией Radis. Значит согласно CAP теореме фокусируется на тех же характеристиках, что и Radis, то есть consistency и partition tolerance. (Про Redis было сказано на лекции)
## ScyllaDB
Scylla предпочитает availability и partition tolerance. Так написано в документации в разделе Scylla Architecture - Fault Tolerance (https://docs.scylladb.com/stable/architecture/architecture-fault-tolerance.html)

## ArenadataDB
На официальном сайте ArenadataDB в ключевых преимуществах выделены дотсупность и консистентность (принципы ACID). С другой стороны логично было бы предположить, что как распределенная база данных, она должна иметь partition tolerance, как одну из ключевых преимуществ. Но раз производитель говорит о ACID, то будем считать, что фокус на consistency и availability (https://arenadata.tech/products/arenadata-db/)
