# 유해물질 법인별 양산보증 측정 현황!

c = (
    Line()
    add_xaxis(Faker.choose())
    add_yaxis("商家A", Faker.values())
    add_yaxis("商家B", Faker.values())
    set_global_opts(title_opts=opts.TitleOpts(title="Line-基本示例"))
    render("line_base.html")
)
