Title: OpenJPA 2.2.0

<a name="OpenJPA2.2.0-OpenJPA2.2.0"></a>

# OpenJPA 2.2.0

The Apache OpenJPA community is proud to announce the release of Apache
OpenJPA 2.2.0.	As with the prior 2.1.0 release, this distribution is based
on the final [JSR 317 Java Persistence API, Version 2.0](http://jcp.org/en/jsr/detail?id=317)
 specification and passes the JPA 2.0 TCK, while remaining backwards
compatible with the prior 1.2.x releases based on the Java Persistence API
(JPA 1.0) part of Java Community Process JSR-220 (Enterprise JavaBeans
3.0).  For a list of all the new features of JPA 2.0, please checkout the [OpenJPA 2.1.0](openjpa-2.1.0.html)
 release notes.

Additional information on the OpenJPA project may be found at [the project web site](http://openjpa.apache.org)
.

<a name="OpenJPA2.2.0-ChangesinOpenJPA2.2.0"></a>

# Changes in OpenJPA 2.2.0

<a name="OpenJPA2.2.0-Sub-task"></a>

### Sub-task
* OPENJPA-1593 - Create an OSGiManagedRuntime
* OPENJPA-2081 - Provide subset of XML support for OpenJPA annotations

<a name="OpenJPA2.2.0-Bug"></a>

### Bug
* OPENJPA-478 - Contradictory text in manual section 10.2.6. JPQL GROUP
BY, HAVING
* OPENJPA-867 - Unexpected Behaviour of DBDictionary.indexOf() method
* OPENJPA-1343 - Incorrect example of openjpa.Sequence property
* OPENJPA-1376 - @SequenceGenerator allocationSize incorrect
implementation
* OPENJPA-1650 - Adding a slice dynamically should be done via
persistence unit only
* OPENJPA-1651 - Unique colums automatically defined as non-nullable
(part 2)
* OPENJPA-1657 - Postgres connection throws NPE with null properties
* OPENJPA-1686 - Persistence of Dynamic and Generic Type
* OPENJPA-1725 - Schemaname wrongly included in
DBDictionary.checkNameLength after Tablename correctly truncated
* OPENJPA-1746 - NullPointerException when a null value is set in the
properties map passed to Entity.createEntityManagerFactory
* OPENJPA-1768 - StackOverflowError when finding an Entity with an
Eager ManyToMany relationship.
* OPENJPA-1787 - Bean validation fails merging a new entity
* OPENJPA-1845 - the prepared query cache doesn't currently work
correclty with 'SELECT IN' statements
* OPENJPA-1856 - Executing bulk updates should evict stale data from
the DataCache
* OPENJPA-1873 - EntityManager#merge sometimes passes wrong entity
values to @PostLoad EntityListeners
* OPENJPA-1876 - Slow JDBC tests
* OPENJPA-1896 - OpenJPA cannot store POJOs if a corresponding record
already exists
* OPENJPA-1898 - TestQueryMultiThreaded fails with OOME "unable to
create new native thread"
* OPENJPA-1900 - ClassCastException when serializing an entity if
DetachedStateField=true
* OPENJPA-1901 - QueryCacheStoreQuery$CachedObjectId that is not
Serializable
* OPENJPA-1902 - SQLServer reserved words may not be used as
identifiers
* OPENJPA-1903 - Some queries only work the first time they are
executed
* OPENJPA-1904 - OptimisticLockException during
refresh(*,PESSIMISTIC_*) with eagar fetch on relationship fields
* OPENJPA-1905 - jar-file validation should be deferred until after
OpenJPA is confirmed to be the application's chosen provider
* OPENJPA-1906 - Issue info / warning message when connection retain
mode is always
* OPENJPA-1909 - enhance unit tests with the correct persistence.xml
* OPENJPA-1910 - openjpa uses application ClassLoader for resolving
BrokerFactory (revisited)
* OPENJPA-1911 - InvalidStateException is thrown when merge an entity
with derived identiy
* OPENJPA-1912 - enhancer generates invalid code if fetch-groups is
activated
* OPENJPA-1915 - missing license header
* OPENJPA-1918 - MetaDataRepository.preload() ignores class loader
returned by PersistenceUnitInfo.getClassLoader()
* OPENJPA-1923 - Allow flexible (non-standard) syntax for
collection-valued parameters in IN() expresseion of JPQL query
* OPENJPA-1928 - Resolving factory method does not allow method
overriding
* OPENJPA-1932 - Documentation corrections
* OPENJPA-1935 - Informix lock exceptions are not mapped properly by
OpenJPA
* OPENJPA-1938 - Typo of time data type in SQLServerdictionary for
MSSQL 2008
* OPENJPA-1939 - index identifier max length for DB2 v9 is 128.
* OPENJPA-1940 - ReverseMapping tool does not find primary keys with
Oracle
* OPENJPA-1941 - Criteria query returns wrong result when query cache
is enabled
* OPENJPA-1943 - Query timeout hint not honored consistently when
pessimistic lock is issued to database requires multi-statements locking
scheme
* OPENJPA-1944 - Extra select statements executed when version column
is null.
* OPENJPA-1951 - missing key "cant-set-value" in localizer properties
org.apache.openjpa.jdbc.meta.strats
* OPENJPA-1953 - Copying data from inputStream to OuputStream needs
appropriate buffer size
* OPENJPA-1954 - ArrayIndexOutOfBoundsException when querying on a
version field that is in a MappedSuperclass
* OPENJPA-1957 - XML overriding column names for ArrayList attributes
causes exception.
* OPENJPA-1958 - IndexOutOfBoundsException in
BatchingPreparedStatementManagerImpl
* OPENJPA-1959 - RuntimeExceptionTranslator should be transient in
DelegatingQuery
* OPENJPA-1960 - openjpa.InitializeEagerly breaks bean-validation
integration
* OPENJPA-1965 - ClassCastException when using JAXB and MetaModel
annotation processor
* OPENJPA-1968 - SQLServerDictionery not using DATETIME2 for jdbc
driver other than MS JDBC driver
* OPENJPA-1969 - SQLServer / DataDirect SQLCode=HYT00 not handled
* OPENJPA-1974 - StackOverflowError when performing multiple subquery
in collection field with eager fetch
* OPENJPA-1975 - Only obtain default schema name when needed (DB2)
* OPENJPA-1981 - Improper cleanup in SchemaGenerator
* OPENJPA-1983 - Merge of lazily fetched fields, and merge of managed
entities deviates from spec
* OPENJPA-1984 - Incorrect ViolationContraint getRootBean when removing
bean with embedded entity validation
* OPENJPA-1985 - ClassCastException in max(Timestamp) function on
PostgreSQL
* OPENJPA-1986 - Extra queries being generated when cascading a persist
* OPENJPA-1987 - Postgres / Ingres does not support null table for
getImportedKeys
* OPENJPA-1989 - *ToOne relationships specified as LAZY in xml aren't
honored
* OPENJPA-1992 - java.lang.ArrayIndexOutOfBoundsException if positional
parameter are not started from 1
* OPENJPA-1994 - Index is a reserved word for MySQL
* OPENJPA-1996 - OpenJPA Samples fail on MacOS X
* OPENJPA-1998 - NPE getTableNameForMetadata when running SchemaTool
reflect against Postgres DB
* OPENJPA-2000 - Wrong PostgreSQL data type for REAL - "float8", must
be "float4"
* OPENJPA-2005 - PostgresDictionary.isOwnedSequence needs a null check
* OPENJPA-2006 - Sequence generated ids may fail to get assigned when
flushing a graph with bi-directional relationships
* OPENJPA-2007 - Setting query hint "openjpa.FetchPlan.Isolation"
results in misleading warning
* OPENJPA-2008 - OpenJPA does not work with native queries in a
distributed (Slice) environment
* OPENJPA-2010 - Duplicate meta data warning logged due to parsing the
same location twice
* OPENJPA-2011 - Prevent reparsing annotation metadata for queries
* OPENJPA-2013 - columnDefinition for TEXT types ends up in wrong sql
statement
* OPENJPA-2025]
 - Byte[](.html) and Char[ should be treated as SingularAttributes, not lists by
the metamodel generator
* OPENJPA-2027 - Metamodel genereated at runtime expects ListAttribute
for all arrays - not just PersistentCollections.
* OPENJPA-2034 - Update H2 Database sql error codes as per the changes
in v1.3.154
* OPENJPA-2036 - DynamicEnhancer should look for tools.jar in
java.home/lib for all JDKs, not just the IBM SDK.
* OPENJPA-2039 - FKs for EAGER fields that are not in the current
fetchplan aren't selected
* OPENJPA-2044 - Invalid header in MetaModel classes generated by
AnnotationProcessor
* OPENJPA-2045 - NAME is a valid column name for H2 databases.
* OPENJPA-2051 - Entities in a relationship are not properly cascaded
after a EntityManager.flush is executed.
* OPENJPA-2056 - Postgres V9.1 issue with LIKE clause and Escape
Strings
* OPENJPA-2059 - Missing localizer.properties for
org.apache.openjpa.persistence.util.SourceCode
* OPENJPA-2060]
 - AnnotationProcess failed to generate metadata for List<String>[
attribute in entity
* OPENJPA-2065 - JPA 2.0 Spec. Violation?
EntityManager#createNamedQuery(String, Class) bombs with non-entity Class
parameter
* OPENJPA-2066 - Edge case in openJPA-1227. openJPA fails to create a
join and thus returns wrong data when a collection is selected from
superclass and another field is selected from subclass twoor more levels
down the hierarchy.
* OPENJPA-2069 - Natvie sequence problems uncovered after OPENJPA-1376
* OPENJPA-2070 - Error processing while populating Metamodel classes
needs improvement
* OPENJPA-2071 - NPE during ResultPacker interface processing
* OPENJPA-2073 - MappingTools requires live connection to DB2 server to
retrieve default schema name
* OPENJPA-2076 - Minor fix-ups to messages
* OPENJPA-2077 - Pom references to org.codehaus.mojo
openjpa-maven-plugin cause problems
* OPENJPA-2083 - Unmapped fields silently treated as transient
* OPENJPA-2100 - openjpa-maven-plugin fails to create SQL for entities
which contain enums
* OPENJPA-2101 - PersistenceProductDerivation overwrites the
RemoteCommitProvider configuration
* OPENJPA-2104 - BindParameter is not a valid query parameter as
processed in DBDictionary's setUnknown()
* OPENJPA-2105 - Document changes no longer being uploaded
* OPENJPA-2107 - ManagedCache conflict due adding an entity 2 times in
the same query.
* OPENJPA-2117 - XML overriding column names for 1xM attributes causes
exception.
* OPENJPA-2119 - Update org.apache.openjpa.persistence.util.SourceCode
* OPENJPA-2122 - VerifyError with Java 7 when using javaagent or
dynamic container enhancement
* OPENJPA-2124 - Use of XMLValueHandler results in a
NullPointerException when classloader does not provide package support

<a name="OpenJPA2.2.0-Improvement"></a>

### Improvement
* OPENJPA-302 - PCEnhancer needs target classes on classpath
* OPENJPA-487 - Generated SUBSTRING SQL is ugly and inefficient
* OPENJPA-758 - OpenJPA doesn't find ValueHandlers with an applicable
class loader
* OPENJPA-1555 - SQLBuffer code cleanup
* OPENJPA-1777 - Allow setting of diagonstic context for each slice in
a more flexible manner
* OPENJPA-1778 - Improved error information for unenhanced classes.
* OPENJPA-1798 - Improve messages in localize.properties
* OPENJPA-1803 - Unwrap EntityManager to Connection
* OPENJPA-1847 - Use a single connection when generating schema
* OPENJPA-1863 - update HSQL dictionary for HSQLDB 2.0
* OPENJPA-1917 - Cache column alias in SelectImpl
* OPENJPA-1937 - Document OpenJPAEntityManager.evict methods
* OPENJPA-1945 - Improve aspects of the OpenBooks sample
* OPENJPA-1972 - DB2 V9.7 changed the default behavior concerning
blocking behavior with isolation levels greater then read uncommitted
* OPENJPA-1990 - Skip getting extend exception text when running on DB2
* OPENJPA-1999 - Optional support for non-sequential positional
parameters
* OPENJPA-2014 - Allow proxies to stay in place when Detaching
* OPENJPA-2020 - Make some members of StateManagerImpl protected to
allow for greater extensability
* OPENJPA-2031 - Unable to import maven projects with m2e version 1.0
* OPENJPA-2042 - Diagnostics for Application Managed
EntityManagerFactory leaks.
* OPENJPA-2043 - OpenJPAId hashCode() value needs to be consistent
after serialization process
* OPENJPA-2047 - Document the impact of Persistence Aware classes
* OPENJPA-2068 - Improve performance of java.util.Calendar fields
* OPENJPA-2075 - Abstract out parameter handling / validation from
org.apache.openjpa.persistence.QueryImpl to allow for greater extensibility
* OPENJPA-2084 - Upgrade Derby dependency to 10.8.x
* OPENJPA-2085 - Improve enhancement process to support JAVA 7
compliant class file generation
* OPENJPA-2087 - Remove or limit the use of the ConcreteClassGenerator
* OPENJPA-2116 - Scrape the barrel for performance juice
* OPENJPA-2120 - Add new option to eliminate reflection calls from
enhancer generated IdClass PC copy operations
* OPENJPA-2128 - Add a boolean to FieldMetaData to denote whether or
not a field has a @EmbeddedId annotation.
* OPENJPA-2130 - Enable Java 7 testing by allowing test cases to
compile targeting to 1.7

<a name="OpenJPA2.2.0-NewFeature"></a>

### New Feature
* OPENJPA-184 - use DB2 Diagnostic interface to report extended error
diagnostics on SQL Exception
* OPENJPA-1859 - Create a sample to demonstrate usage of JEST
* OPENJPA-1934 - contribute an openjpa-maven-plugin
* OPENJPA-2108 - Allow an option to terminate MappingTool-generated SQL
with a character other than semicolon

<a name="OpenJPA2.2.0-Task"></a>

### Task
* OPENJPA-1786 - Upgrade to latest JPA 2.0 TCK
* OPENJPA-1834 - Upgrade trunk to use Deby 10.6.2.1 for junits
* OPENJPA-1875 - Add generics to the Graph code
* OPENJPA-2089 - upgrade bval to latest 0.3-incubating
* OPENJPA-2091 - update docbook maven plugin

<a name="OpenJPA2.2.0-Test"></a>

### Test
* OPENJPA-2029 - Add PreparedQuery tests for non-sequential positional
parameters support
