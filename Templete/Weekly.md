# {{date:Y ww}}

> [!multi-column]
> 
> > [!note]+ 大事记
> > 
> > 1. <% tp.file.cursor(1) %>
> 
> > [!note]+ 随想录
> > 
> > <% tp.file.cursor(2) %>

## 本周日记

```dataview
table without id
file.link as "日期", dateformat(date(file.name, "yyyy.LL.dd"), "cccc") as "星期"
where string(dateformat(date(file.name, "yyyy.LL.dd"), "yyyy WW")) = this.file.name
sort file.name asc
```