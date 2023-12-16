@RestController
@RequestMapping("/api/v1/servicio-taxi")
@Api(value = "Servicio de Taxi", tags = "Servicio de Taxi")
public class ServicioTaxiController {

    @ApiOperation(value = "Registrar solicitud de servicio de taxi", response = ResponseEntity.class)
    @ApiResponses(value = {
            @ApiResponse(code = 200, message = "Solicitud registrada exitosamente"),
            @ApiResponse(code = 400, message = "Solicitud inválida"),
            @ApiResponse(code = 500, message = "Error interno en el servidor")
    })
    @PostMapping("/registrar-solicitud")
    public ResponseEntity<String> registrarSolicitud(@RequestBody SolicitudTaxi solicitud) {
        
    }
}

 
