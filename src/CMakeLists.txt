add_executable(Raytracing)

target_sources(Raytracing PRIVATE
	main.cpp
	ray.h
	color.h
	vec3.h
	hittable.h
	hittable_list.h
	sphere.h
	rtweekend.h
	interval.h
	camera.h
	material.h
)