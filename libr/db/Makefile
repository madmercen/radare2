include ../config.mk

NAME=r_db
DEPS=r_util

OBJS=db.o table.o pair.o

SDBPATH=../../shlr/sdb/src/
SDBLIB=${SDBPATH}/libsdb.a
EXTRA_TARGETS+=${SDBLIB}
SDB_OBJS=
SDB_OBJS+=buffer.o
SDB_OBJS+=cdb.o
SDB_OBJS+=cdb_make.o
SDB_OBJS+=ht.o
SDB_OBJS+=json/js0n.o
SDB_OBJS+=json/json.o
SDB_OBJS+=json/rangstr.o
SDB_OBJS+=json.o
SDB_OBJS+=lock.o
SDB_OBJS+=ls.o
SDB_OBJS+=ns.o
SDB_OBJS+=query.o
SDB_OBJS+=sdb.o
SDB_OBJS+=sdba.o
SDB_OBJS+=sdbn.o
SDB_OBJS+=util.o

SDBOBJS=$(addprefix ${SDBPATH},${SDB_OBJS})

OBJS+=${SDBOBJS}

CFLAGS+=-I${SDBPATH}/src

include ../rules.mk
