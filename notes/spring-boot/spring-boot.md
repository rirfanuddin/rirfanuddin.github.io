# Spring Boot

### create pageable from list
we have ``List<User> list`` data and create a _pageable_ response
```
Pageable pageable = PageRequest.of(0, 10);
int start = (int) pageable.getOffset();
inst end = (int) (start + pageable.getPageSize()) > list.size() ? list.size() : (start + pageable.getPageSize());
Page<User> response = new PageImpl<User>(list.subList(start, end), pageable, list.size());
return response; 
```